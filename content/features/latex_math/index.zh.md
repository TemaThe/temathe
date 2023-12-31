---
title: "LaTex Math Support"
date: "2023-10-22T21:24:55+08:00"
author: "KaTex Doc"
tags: ["lartex", "example", "math"]
categories: ["feature", "latex"]
description: "Example page to demonstrate the support of LaTex"
keywords: "latex,example,math"
localCss: ["no_thead.css", "latex_demo.css"]
useMath: true
---

> The content in this page is copied from the [KaTeX Official Supported Functions](https://katex.org/docs/supported.html) page.
> I have only made some changes to fit the migration with the Hugo system.

## Accents

|                |                |                            |                            |                         |                         |
| :------------- | :------------- | :------------------------- | :------------------------- | :---------------------- | :---------------------- |
| $a'$           | `a'`           | $\tilde{a}$                | `\tilde{a}`                | $\mathring{g}$          | `\mathring{g}`          |
| $a''$          | `a''`          | $\widetilde{ac}$           | `\widetilde{ac}`           | $\overgroup{AB}$        | `\overgroup{AB}`        |
| $a^{\prime}$   | `a^{\prime}`   | $\utilde{AB}$              | `\utilde{AB}`              | $\undergroup{AB}$       | `\undergroup{AB}`       |
| $\acute{a}$    | `\acute{a}`    | $\vec{F}$                  | `\vec{F}`                  | $\Overrightarrow{AB}$   | `\Overrightarrow{AB}`   |
| $\bar{y}$      | `\bar{y}`      | $\overleftarrow{AB}$       | `\overleftarrow{AB}`       | $\overrightarrow{AB}$   | `\overrightarrow{AB}`   |
| $\breve{a}$    | `\breve{a}`    | $\underleftarrow{AB}$      | `\underleftarrow{AB}`      | $\underrightarrow{AB}$  | `\underrightarrow{AB}`  |
| $\check{a}$    | `\check{a}`    | $\overleftharpoon{ac}$     | `\overleftharpoon{ac}`     | $\overrightharpoon{ac}$ | `\overrightharpoon{ac}` |
| $\dot{a}$      | `\dot{a}`      | $\overleftrightarrow{AB}$  | `\overleftrightarrow{AB}`  | $\overbrace{AB}$        | `\overbrace{AB}`        |
| $\ddot{a}$     | `\ddot{a}`     | $\underleftrightarrow{AB}$ | `\underleftrightarrow{AB}` | $\underbrace{AB}$       | `\underbrace{AB}`       |
| $\grave{a}$    | `\grave{a}`    | $\overline{AB}$            | `\overline{AB}`            | $\overlinesegment{AB}$  | `\overlinesegment{AB}`  |
| $\hat{\theta}$ | `\hat{\theta}` | $\underline{AB}$           | `\underline{AB}`           | $\underlinesegment{AB}$ | `\underlinesegment{AB}` |
| $\widehat{ac}$ | `\widehat{ac}` | $\widecheck{ac}$           | `\widecheck{ac}`           | $\underbar{X}$          | `\underbar{X}`          |

### Accent functions inside `\\text{...}`

|                 |             |                |         |                |         |                |         |
| :-------------- | :---------- | :------------- | :------ | :------------- | :------ | :------------- | :------ |
| $\text{\'{a}}$  | `\'{a}`     | $\text{\~{a}}$ | `\~{a}` | $\text{\.{a}}$ | `\.{a}` | $\text{\H{a}}$ | `\H{a}` |
| $\text{\`{a}}$  | ``\`{a}``  | $\text{\={a}}$ | `\={a}` | $\text{\"{a}}$ | `\"{a}` | $\text{\v{a}}$ | `\v{a}` |
| $\text{\\^{a}}$ | `\\^{a}`    | $\text{\u{a}}$ | `\u{a}` | $\text{\r{a}}$ | `\r{a}` |

* See also [letters and unicode](#letters-and-unicode).

## Delimiters

| Symbol          | Syntax 1          | Syntax 2                  | Symbol            | Syntax 1          | Syntax 2                  |
| :-------------- | :---------------- | :------------------------ | :---------------- | :---------------- | :------------------------ |
| $(~)$           | `( )`             | `\lparen \rparen`         | $⌈~⌉$             | `⌈ ⌉`             | `\lceil \rceil`           |
| $[~]$           | `[ ]`             | `\lbrack \rbrack`         | $⌊~⌋$             | `⌊ ⌋`             | `\lfloor \rfloor`         |
| $\\{ \\}$       | `\\{ \\}`         | `\lbrace \rbrace`         | $⎰⎱$              | `⎰ ⎱`             | `\lmoustache \rmoustache` |
| $⟨~⟩$           | `⟨ ⟩`             | `\langle \rangle`         | $⟮~⟯$             | `⟮ ⟯`             | `\lgroup \rgroup`         |
| $┌ ┐$           | `┌ ┐`             | `\ulcorner \urcorner`     | $└ ┘$             | `└ ┘`             | `\llcorner \lrcorner`     |
| $\vert$         | `\|`              | `\vert`                   | $\Vert$           | `∥`               | `\Vert`                   |
| $⟦~⟧$           | `⟦` `⟧`           | `\llbracket` `\rrbracket` | $\lBrace~\rBrace$ | `\lBrace \rBrace` |                           |
| $\lvert~\rvert$ | `\lvert` `\rvert` |                           | $\lVert~\rVert$   | `\lVert` `\rVert` |
| $\lang~\rang$   | `\lang` `\rang`   |                           | $\lt~\gt$         | `\lt` `\gt`       |                           |
| $\backslash$    | `\backslash`      |                           |                   |                   |                           |
| $\downarrow$    | `\downarrow`      |                           | $\Downarrow$      | `\Downarrow`      |                           |
| $\uparrow$      | `\uparrow`        |                           | $\Uparrow$        | `\Uparrow`        |                           |
| $\updownarrow$  | `\updownarrow`    |                           | $\Updownarrow$    | `\Updownarrow`    |                           |

### Delimiter Sizing

* $\left(\LARGE{AB}\right)$ `\left(\LARGE{AB}\right)`
* $( \big( \Big( \bigg( \Bigg($ `( \big( \Big( \bigg( \Bigg(`

|           |         |          |          |          |
| :-------- | :------ | :------- | :------- | :------- |
| `\left`   | `\big`  | `\bigl`  | `\bigm`  | `\bigr`  |
| `\middle` | `\Big`  | `\Bigl`  | `\Bigm`  | `\Bigr`  |
| `\right`  | `\bigg` | `\biggl` | `\biggm` | `\biggr` |
|           | `\Bigg` | `\Biggl` | `\Biggm` | `\Biggr` |

## Environments

<table class="latex-demo">
    <tr>
        <td>$\begin{matrix} a & b \\ c & d \end{matrix}$</td>
        <td><pre><code>\begin{matrix}
    a & b \\\\
    c & d
\end{matrix}</code></pre></td>
        <td>$\begin{array}{cc}a & b \\ c & d \end{array}$</td>
        <td><pre><code>\begin{array}{cc}
    a & b \\\\
    c & d
\end{array}</code></pre></td>
    </tr>
    <tr>
        <td>$\begin{pmatrix} a & b \\ c & d \end{pmatrix}$</td>
        <td><pre><code>\begin{pmatrix}
    a & b \\\\
    c & d
\end{pmatrix}</code></pre></td>
        <td>$\begin{bmatrix} a & b \\ c & d \end{bmatrix}$</td>
        <td><pre><code>\begin{bmatrix}
    a & b \\\\
    c & d
\end{bmatrix}</code></pre></td>
    </tr>
    <tr>
        <td>$\begin{vmatrix} a & b \\ c & d \end{vmatrix}$</td>
        <td><pre><code>\begin{vmatrix}
    a & b \\\\
    c & d
\end{vmatrix}</code></pre></td>
        <td>$\begin{Vmatrix} a & b \\ c & d \end{Vmatrix}$</td>
        <td><pre><code>\begin{Vmatrix}
    a & b \\\\
    c & d
\end{Vmatrix}</code></pre></td>
    </tr>
    <tr>
        <td>$\begin{Bmatrix} a & b \\ c & d \end{Bmatrix}$</td>
        <td><pre><code>\begin{Bmatrix}
    a & b \\\\
    c & d
\end{Bmatrix}</code></pre></td>
        <td>$\def\arraystretch{1.5}\begin{array}{c:c:c} a & b & c \\ \hline d & e & f \\ \hdashline g & h & i \end{array}$</td>
        <td><pre><code>\def\arraystretch{1.5}
\begin{array}{c:c:c}
                    a & b & c \\\
        \hline      d & e & f \\\
        \hdashline  g & h & i
\end{array}</code></pre></td>
    </tr>
    <tr>
        <td>$x = \begin{cases} a & \text{if } b \\ c & \text{if } d \end{cases}$</td>
        <td><pre><code>x = \begin{cases}
   a & \\text{if } b \\\\
   c & \\text{if } d
\end{cases}</code></pre></td>
        <td>$\begin{rcases} a &\text{if } b \\ c &\text{if } d \end{rcases}⇒...$</td>
        <td><pre><code>\begin{rcases}
   a & \\text{if } b \\\\
   c & \\text{if } d
\end{rcases}⇒...</code></pre></td>
    </tr>
    <tr>
        <td>$\begin{smallmatrix} a & b \\ c & d \end{smallmatrix}$</td>
        <td><pre><code>\begin{smallmatrix}
    a & b \\\\
    c & d
\end{smallmatrix}</code></pre></td>
        <td>$$\sum_{\begin{subarray}{l} i\in\Lambda\\  0&lt;j&lt;n\end{subarray}}$$</td>
        <td><pre><code>\sum_{
    \begin{subarray}{l}
        i \\in \\Lambda \\\\
        0 < j < n
    \end{subarray}
}</code></pre></td>
    </tr>
</table>

* The auto-render extension will render the following environments even if they are not inside math delimiters such as `$...$`. They are display-mode only.

<table class="latex-demo env-auto-gen">
    <tr>
        <td>\begin{equation}\begin{split}a &=b+c \\ &=e+f \end{split}\end{equation}</td>
        <td><pre><code>\begin{equation}
    \begin{split}
        a & = b + c \\
          & = e + f
    \end{split}
\end{equation}</code></pre></td>
        <td>\begin{align} a&=b+c \\ d+e&=f \end{align}</td>
        <td><pre><code>\begin{align}
        a &= b + c \\
    d + e &=f
\end{align}</code></pre></td>
    </tr>
    <tr>
        <td> \begin{gather} a=b \\ e=b+c \end{gather}</td>
        <td><pre><code> \begin{gather}
    a = b       \\
    e = b + c
\end{gather}</code></pre></td>
        <td>\begin{alignat}{2} 10&x+&3&y=2 \\ 3&x+&13&y=4 \end{alignat}</td>
        <td><pre><code>\begin{alignat}{2}
    10 & x + &  3 & y = 2   \\
     3 & x + & 13 & y = 4
\end{alignat}</code></pre></td>
    </tr>
    <tr>
        <td>\begin{CD} A @>a>> B \\ @VbVV @AAcA \\ C @= D \end{CD}</td>
        <td><pre><code>\begin{CD}
    A @>a>> B   \\
    @VbVV @AAcA \\
    C @= D
\end{CD}</code></pre></td>
        <td></td>
        <td></td>
    </tr>
</table>

### Other KaTeX Environments

| Environments                                                          | How they differ from those shown above                                                                                                                                  |
| :-------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `darray`, `dcases`, `drcases`                                         | apply `displaystyle`                                                                                                                                                    |
| `matrix*`, `pmatrix*`, `bmatrix*`, `Bmatrix*`, `vmatrix*`, `Vmatrix*` | take an optional argument to set column alignment, as in `\begin{matrix*}[r]`                                                                                           |
| `equation*`, `gather*`, `align*`, `alignat*`                          | have no automatic numbering. Alternatively, you can use `\nonumber` or `\notag` to omit the numbering for a specific row of the equation.                               |
| `gathered`, `aligned`, `alignedat`                                    | 1. do not need to be in display mode. <br> 2. have no automatic numbering. <br> 3. must be inside math delimiters in order to be rendered by the auto-render extension. |

* Acceptable line separators include: `\\\\`, `\cr`, `\\\\[distance]`, and `\cr[distance]`. *Distance* can be written with any of the [KaTeX units](#units).
* The `{array}` environment supports `|` and `:` vertical separators.
* The `{array}` environment does not yet support `\cline` or `\multicolumn`.
* `\tag` can be applied to individual rows of top-level environments (`align`, `align*`, `alignat`, `alignat*`, `gather`, `gather*`).

## Letters and Unicode

### Greek Letters

* Direct Input: $Α Β Γ Δ Ε Ζ Η Θ Ι \allowbreak Κ Λ Μ Ν Ξ Ο Π Ρ Σ Τ Υ Φ Χ Ψ Ω$
$\allowbreak α β γ δ ϵ ζ η θ ι κ λ μ ν ξ o π \allowbreak ρ σ τ υ ϕ χ ψ ω ε ϑ ϖ ϱ ς φ ϝ$

|                             |                         |                         |                             |
| --------------------------- | ----------------------- | ----------------------- | --------------------------- |
| $\Alpha$ `\Alpha`           | $\Beta$ `\Beta`         | $\Gamma$ `\Gamma`       | $\Delta$ `\Delta`           |
| $\Epsilon$ `\Epsilon`       | $\Zeta$ `\Zeta`         | $\Eta$ `\Eta`           | $\Theta$ `\Theta`           |
| $\Iota$ `\Iota`             | $\Kappa$ `\Kappa`       | $\Lambda$ `\Lambda`     | $\Mu$ `\Mu`                 |
| $\Nu$ `\Nu`                 | $\Xi$ `\Xi`             | $\Omicron$ `\Omicron`   | $\Pi$ `\Pi`                 |
| $\Rho$ `\Rho`               | $\Sigma$ `\Sigma`       | $\Tau$ `\Tau`           | $\Upsilon$ `\Upsilon`       |
| $\Phi$ `\Phi`               | $\Chi$ `\Chi`           | $\Psi$ `\Psi`           | $\Omega$ `\Omega`           |
| $\varGamma$ `\varGamma`     | $\varDelta$ `\varDelta` | $\varTheta$ `\varTheta` | $\varLambda$ `\varLambda`   |
| $\varXi$ `\varXi`           | $\varPi$ `\varPi`       | $\varSigma$ `\varSigma` | $\varUpsilon$ `\varUpsilon` |
| $\varPhi$ `\varPhi`         | $\varPsi$ `\varPsi`     | $\varOmega$ `\varOmega` |                             |
| $\alpha$ `\alpha`           | $\beta$ `\beta`         | $\gamma$ `\gamma`       | $\delta$ `\delta`           |
| $\epsilon$ `\epsilon`       | $\zeta$ `\zeta`         | $\eta$ `\eta`           | $\theta$ `\theta`           |
| $\iota$ `\iota`             | $\kappa$ `\kappa`       | $\lambda$ `\lambda`     | $\mu$ `\mu`                 |
| $\nu$ `\nu`                 | $\xi$ `\xi`             | $\omicron$ `\omicron`   | $\pi$ `\pi`                 |
| $\rho$ `\rho`               | $\sigma$ `\sigma`       | $\tau$ `\tau`           | $\upsilon$ `\upsilon`       |
| $\phi$ `\phi`               | $\chi$ `\chi`           | $\psi$ `\psi`           | $\omega$ `\omega`           |
| $\varepsilon$ `\varepsilon` | $\varkappa$ `\varkappa` | $\vartheta$ `\vartheta` | $\thetasym$ `\thetasym`     |
| $\varpi$ `\varpi`           | $\varrho$ `\varrho`     | $\varsigma$ `\varsigma` | $\varphi$ `\varphi`         |
| $\digamma $ `\digamma`

### Other Letters

|                       |                       |                       |                           |                           |
| :-------------------- | :-------------------- | :-------------------- | :------------------------ | :------------------------ |
| $\imath$ `\imath`     | $\nabla$ `\nabla`     | $\Im$ `\Im`           | $\Reals$ `\Reals`         | $\text{\OE}$ `\text{\OE}` |
| $\jmath$ `\jmath`     | $\partial$ `\partial` | $\image$ `\image`     | $\wp$ `\wp`               | $\text{\o}$ `\text{\o}`   |
| $\aleph$ `\aleph`     | $\Game$ `\Game`       | $\Bbbk$ `\Bbbk`       | $\weierp$ `\weierp`       | $\text{\O}$ `\text{\O}`   |
| $\alef$ `\alef`       | $\Finv$ `\Finv`       | $\N$ `\N`             | $\Z$ `\Z`                 | $\text{\ss}$ `\text{\ss}` |
| $\alefsym$ `\alefsym` | $\cnums$ `\cnums`     | $\natnums$ `\natnums` | $\text{\aa}$ `\text{\aa}` | $\text{\i}$ `\text{\i}`   |
| $\beth$ `\beth`       | $\Complex$ `\Complex` | $\R$ `\R`             | $\text{\AA}$ `\text{\AA}` | $\text{\j}$ `\text{\j}`   |
| $\gimel$ `\gimel`     | $\ell$ `\ell`         | $\Re$ `\Re`           | $\text{\ae}$ `\text{\ae}` |                           |
| $\daleth$ `\daleth`   | $\hbar$ `\hbar`       | $\real$ `\real`       | $\text{\AE}$ `\text{\AE}` |                           |
| $\eth$ `\eth`         | $\hslash$ `\hslash`   | $\reals$ `\reals`     | $\text{\oe}$ `\text{\oe}` |                           |

* Direct Input: $∂ ∇ ℑ Ⅎ ℵ ℶ ℷ ℸ ⅁ ℏ ð − ∗$
ÀÁÂÃÄÅÆÇÈÉÊËÌÍÎÏÐÑÒÓÔÕÖÙÚÛÜÝÞßàáâãäåçèéêëìíîïðñòóôöùúûüýþÿ
₊₋₌₍₎₀₁₂₃₄₅₆₇₈₉ₐₑₕᵢⱼₖₗₘₙₒₚᵣₛₜᵤᵥₓᵦᵧᵨᵩᵪ⁺⁻⁼⁽⁾⁰¹²³⁴⁵⁶⁷⁸⁹ᵃᵇᶜᵈᵉᵍʰⁱʲᵏˡᵐⁿᵒᵖʳˢᵗᵘʷˣʸᶻᵛᵝᵞᵟᵠᵡ

* Math-mode Unicode (sub|super)script characters will render as if you had written regular characters in a subscript or superscript. For instance, `A²⁺³` will render the same as `A^{2+3}`.

### Unicode Mathematical Alphanumeric Symbols

| Item         | Range                   | Item              | Range                |
| ------------ | ----------------------- | ----------------- | -------------------- |
| Bold         | $\text{𝐀-𝐙 𝐚-𝐳 𝟎-𝟗}$    | Double-struck     | $\text{𝔸-}ℤ\ 𝕜$      |
| Italic       | $\text{𝐴-𝑍 𝑎-𝑧}$        | Sans serif        | $\text{𝖠-𝖹 𝖺-𝗓 𝟢-𝟫}$ |
| Bold Italic  | $\text{𝑨-𝒁 𝒂-𝒛}$        | Sans serif bold   | $\text{𝗔-𝗭 𝗮-𝘇 𝟬-𝟵}$ |
| Script       | $\text{𝒜-𝒵}$            | Sans serif italic | $\text{𝘈-𝘡 𝘢-𝘻}$     |
| Fractur      | $\text{𝔄-ℨ}\text{ 𝔞-𝔷}$ | Monospace         | $\text{𝙰-𝚉 𝚊-𝚣 𝟶-𝟿}$ |
| Bold Fractur | $\text{𝕬-𝖅}\text{𝖆-𝖟}$  |                   |                      |

### Unicode

* The letters listed above will render properly in any KaTeX rendering mode.
* In addition, Armenian, Brahmic, Georgian, Chinese, Japanese, and Korean glyphs are always accepted in text mode. However, these glyphs will be rendered from system fonts (not KaTeX-supplied fonts) so their typography may clash.
* You can provide rules for CSS classes `.latin_fallback`, `.cyrillic_fallback`, `.brahmic_fallback`, `.georgian_fallback`, `.cjk_fallback`, and `.hangul_fallback` to provide fallback fonts for these languages.
* Use of these glyphs may cause small vertical alignment issues: KaTeX has detailed metrics for listed symbols and most Latin, Greek, and Cyrillic letters, but other accepted glyphs are treated as if they are each as tall as the letter M in the current KaTeX font.
* If the KaTeX rendering mode is set to `strict: false` or `strict: "warn"` (default), then KaTeX will accept all Unicode letters in both text and math mode.
* All unrecognized characters will be treated as if they appeared in text mode, and are subject to the same issues of using system fonts and possibly using incorrect vertical alignment.
* For Persian composite characters, a user-supplied [plug-in](https://github.com/HosseinAgha/persian-katex-plugin) is under development.
* Any character can be written with the `\char` function and the Unicode code in hex. For example `\char"263a` will render as $\char"263a$.

## Layout

### Annotation

|                       |                     |                                    |                                    |
| :-------------------- | :------------------ | :--------------------------------- | :--------------------------------- |
| $\cancel{5}$          | `\cancel{5}`        | $\overbrace{a+b+c}^{\text{note}}$  | `\overbrace{a+b+c}^{\text{note}}`  |
| $\bcancel{5}$         | `\bcancel{5}`       | $\underbrace{a+b+c}_{\text{note}}$ | `\underbrace{a+b+c}_{\text{note}}` |
| $\xcancel{ABC}$       | `\xcancel{ABC}`     | $\not =$                           | `\not =`                           |
| $\sout{abc}$          | `\sout{abc}`        | $\boxed{\pi=\frac c d}$            | `\boxed{\pi=\frac c d}`            |
| $a_{\angl n}$         | `$a_{\angl n}`      | $a_\angln$                         | `a_\angln`                         |
| $\phase{-78^\circ}$   | `\phase{-78^\circ}` |                                    |                                    |

### Tags

* `\tag{hi} x+y^{2x}`

<div class="latex-demo-annotation-table">

|                       |
| :-------------------- |
| $$\tag{hi} x+y^{2x}$$ |

</div>

* `\tag*{hi} x+y^{2x}`

<div class="latex-demo-annotation-table">

|                       |
| :-------------------- |
| $$\tag*{hi} x+y^{2x}$$ |
</div>

### Line Breaks

* KaTeX 0.10.0+ will insert automatic line breaks in inline math after relations or binary operators such as “=” or “+”. These can be suppressed by `\nobreak` or by placing math inside a pair of braces, as in `{F=ma}`. `\allowbreak` will allow automatic line breaks at locations other than relations or operators.
* Hard line breaks are `\\\\` and `\newline`.
* In display math, KaTeX does not insert automatic line breaks. It ignores display math hard line breaks when rendering option `strict: true`.

### Vertical Layout

|         |         |                   |                   |                                              |                                                       |
| :------ | :------ | :---------------- | :---------------- | :------------------------------------------- | :---------------------------------------------------- |
| $x_n$   | `x_n`   | $\stackrel{!}{=}$ | `\stackrel{!}{=}` | $a \atop b$                                  | `a \atop b`                                           |
| $e^x$   | `e^x`   | $\overset{!}{=}$  | `\overset{!}{=}`  | $a\raisebox{0.25em}{$b$}c$                   | `a\raisebox{0.25em}{$b$}c`                            |
| $\_u^o$ | `_u^o` | $\underset{!}{=}$ | `\underset{!}{=}` | $a+\left(\vcenter{\frac{\frac a b}c}\right)$ | `a+\left(\vcenter{\hbox{$\frac{\frac a b}c$}}\right)` |
|         |         |                   |                   | $$\sum_{\substack{0<i<m\\\\0<j<n}}$$         | `\sum_{\substack{0<i<m\\\\0<j<n}}`                    |

* `\raisebox` and `\hbox` put their argument into text mode. To raise math, nest `$...$` delimiters inside the argument as shown above.
* `\vcenter` can be written without an `\hbox` if the `strict` rendering option is *false*. In that case, omit the nested `$...$` delimiters.

### Overlap and Spacing

<table class="latex-demo">
    <tr>
        <td>${=}\mathllap{/\,}$</td>
        <td><code>{=}\mathllap{/\,}</code></td>
        <td>$\left(x^{\smash{2}}\right)$</td>
        <td><code>\left(x^{\smash{2}}\right)</code></td>
    </tr>
    <tr>
        <td>$\mathrlap{\,/}{=}$</td>
        <td><code>\mathrlap{\,/}{=}</code></td>
        <td>$\sqrt{\smash[b]{y}}$</td>
        <td><code>\sqrt{\smash[b]{y}}</code></td>
    </tr>
    <tr>
        <td>$\displaystyle\sum_{\mathclap{1\le i\le j\le n}} x_{ij}$</td>
        <td colspan=3><code>`\sum_{\mathclap{1\le i\le j\le n}} x_{ij}`</code></td>
    </tr>
</table>

* KaTeX also supports `\llap`, `\rlap`, and `\clap`, but they will take only text, not math, as arguments.

#### Spacing

| Function        | Produces           | Function             | Produces                              |
| :-------------- | :----------------- | :------------------- | :------------------------------------ |
| `\,`            | ³∕₁₈ em space      | `\kern{distance}`    | space, width = *distance*             |
| `\thinspace`    | ³∕₁₈ em space      | `\mkern{distance}`   | space, width = *distance*             |
| `\>`            | ⁴∕₁₈ em space      | `\mskip{distance}`   | space, width = *distance*             |
| `\:`            | ⁴∕₁₈ em space      | `\hskip{distance}`   | space, width = *distance*             |
| `\medspace`     | ⁴∕₁₈ em space      | `\hspace{distance}`  | space, width = *distance*             |
| `\;`            | ⁵∕₁₈ em space      | `\hspace*{distance}` | space, width = *distance*             |
| `\thickspace`   | ⁵∕₁₈ em space      | `\phantom{content}`  | space the width and height of content |
| `\enspace`      | ½ em space         | `\hphantom{content}` | space the width of content            |
| `\quad`         | 1 em space         | `\vphantom{content}` | a strut the height of content         |
| `\qquad`        | 2 em space         | `\!`                 | – ³∕₁₈ em space                       |
| `~`             | non-breaking space | `\negthinspace`      | – ³∕₁₈ em space                       |
| `\<space>`      | space              | `\negmedspace`       | – ⁴∕₁₈ em space                       |
| `\nobreakspace` | non-breaking space | `\negthickspace`     | – ⁵∕₁₈ em space                       |
| `\space`        | space              | `\mathstrut`         | `\vphantom{(}`                        |

#### Notes

* `distance` will accept any of the [KaTeX units](#units).
* `\kern`, `\mkern`, `\mskip`, and `\hspace` accept unbraced distances, as in: `\kern1em`.
* `\mkern` and `\mskip` will not work in text mode and both will write a console warning for any unit except `mu`.

## Logic and Set Theory

$\gdef\VERT{|}$

|                       |                                                                              |                                                       |                             |
| :-------------------- | :--------------------------------------------------------------------------- | :---------------------------------------------------- | :-------------------------- |
| $\forall$ `\forall`   | $\complement$ `\complement`                                                  | $\therefore$ `\therefore`                             | $\emptyset$ `\emptyset`     |
| $\exists$ `\exists`   | $\subset$ `\subset`                                                          | $\because$ `\because`                                 | $\empty$ `\empty`           |
| $\exist$ `\exist`     | $\supset$ `\supset`                                                          | $\mapsto$ `\mapsto`                                   | $\varnothing$ `\varnothing` |
| $\nexists$ `\nexists` | $\mid$ `\mid`                                                                | $\to$ `\to`                                           | $\implies$ `\implies`       |
| $\in$ `\in`           | $\land$ `\land`                                                              | $\gets$ `\gets`                                       | $\impliedby$ `\impliedby`   |
| $\isin$ `\isin`       | $\lor$ `\lor`                                                                | $\leftrightarrow$ `\leftrightarrow`                   | $\iff$ `\iff`               |
| $\notin$ `\notin`     | $\ni$ `\ni`                                                                  | $\notni$ `\notni`                                     | $\neg$ `\neg` or `\lnot`    |
|                       | $\Set{ x \VERT x<\frac 1 2 }$ <br> <code>\Set{ x &#124; x<\frac 1 2 }</code> | $\set{x\VERT x<5}$ <br> <code>\set{x&#124;x<5}</code> |                             |

* Direct Input: $∀ ∴ ∁ ∵ ∃ ∣ ∈ ∉ ∋ ⊂ ⊃ ∧ ∨ ↦ → ← ↔ ¬$ ℂ ℍ ℕ ℙ ℚ ℝ

## Macros

|                                       |                                                   |
| :------------------------------------ | :------------------------------------------------ |
| $\def\foo{x^2} \foo + \foo$           | `\def\foo{x^2} \foo + \foo`                       |
| $\gdef\foo#1{#1^2} \foo{y} + \foo{y}$ | `\gdef\foo#1{#1^2} \foo{y} + \foo{y}`             |
|                                       | `\edef\macroname#1#2…{definition to be expanded}` |
|                                       | `\xdef\macroname#1#2…{definition to be expanded}` |
|                                       | `\let\foo=\bar`                                   |
|                                       | `\futurelet\foo\bar x`                            |
|                                       | `\global\def\macroname#1#2…{definition}`          |
|                                       | `\newcommand\macroname[numargs]{definition}`      |
|                                       | `\renewcommand\macroname[numargs]{definition}`    |
|                                       | `\providecommand\macroname[numargs]{definition}`  |

* Macros can also be defined in the KaTeX [rendering options](options.md).
* Macros accept up to nine arguments: #1, #2, etc.
* Macros defined by `\gdef`, `\xdef`, `\global\def`, `\global\edef`, `\global\let`, and `\global\futurelet` will persist between math expressions. (Exception: macro persistence may be disabled. There are legitimate security reasons for that.)
* KaTeX has no `\par`, so all macros are long by default and `\long` will be ignored.
* Available functions include: `\char` `\mathchoice` `\TextOrMath` `\@ifstar` `\@ifnextchar` `\@firstoftwo` `\@secondoftwo` `\relax` `\expandafter` `\noexpand`
* `@` is a valid character for commands, as if `\makeatletter` were in effect.

## Operators

### Big Operators

|                   |                         |                           |                         |
| ----------------- | ----------------------- | ------------------------- | ----------------------- |
| $\sum$ `\sum`     | $\prod$ `\prod`         | $\bigotimes$ `\bigotimes` | $\bigvee$ `\bigvee`     |
| $\int$ `\int`     | $\coprod$ `\coprod`     | $\bigoplus$ `\bigoplus`   | $\bigwedge$ `\bigwedge` |
| $\iint$ `\iint`   | $\intop$ `\intop`       | $\bigodot$ `\bigodot`     | $\bigcap$ `\bigcap`     |
| $\iiint$ `\iiint` | $\smallint$ `\smallint` | $\biguplus$ `\biguplus`   | $\bigcup$ `\bigcup`     |
| $\oint$ `\oint`   | $\oiint$ `\oiint`       | $\oiiint$ `\oiiint`       | $\bigsqcup$ `\bigsqcup` |

* Direct Input: $∫ ∬ ∭ ∮ ∏ ∐ ∑ ⋀ ⋁ ⋂ ⋃ ⨀ ⨁ ⨂ ⨄ ⨆$ ∯ ∰

### Binary Operators

|                         |                                     |                                     |                                       |
| ----------------------- | ----------------------------------- | ----------------------------------- | ------------------------------------- |
| $+$ `+`                 | $\cdot$ `\cdot`                     | $\gtrdot$ `\gtrdot`                 | $x \pmod a$ `x \pmod a`               |
| $-$ `-`                 | $\cdotp$ `\cdotp`                   | $\intercal$ `\intercal`             | $x \pod a$ `x \pod a`                 |
| $/$ `/`                 | $\centerdot$ `\centerdot`           | $\land$ `\land`                     | $\rhd$ `\rhd`                         |
| $*$ `*`                 | $\circ$ `\circ`                     | $\leftthreetimes$ `\leftthreetimes` | $\rightthreetimes$ `\rightthreetimes` |
| $\amalg$ `\amalg`       | $\circledast$ `\circledast`         | $\ldotp$ `\ldotp`                   | $\rtimes$ `\rtimes`                   |
| $\And$ `\And`           | $\circledcirc$ `\circledcirc`       | $\lor$ `\lor`                       | $\setminus$ `\setminus`               |
| $\ast$ `\ast`           | $\circleddash$ `\circleddash`       | $\lessdot$ `\lessdot`               | $\smallsetminus$ `\smallsetminus`     |
| $\barwedge$ `\barwedge` | $\Cup$ `\Cup`                       | $\lhd$ `\lhd`                       | $\sqcap$ `\sqcap`                     |
| $\bigcirc$ `\bigcirc`   | $\cup$ `\cup`                       | $\ltimes$ `\ltimes`                 | $\sqcup$ `\sqcup`                     |
| $\bmod$ `\bmod`         | $\curlyvee$ `\curlyvee`             | $x \mod a$ `x\mod a`                | $\times$ `\times`                     |
| $\boxdot$ `\boxdot`     | $\curlywedge$ `\curlywedge`         | $\mp$ `\mp`                         | $\unlhd$ `\unlhd`                     |
| $\boxminus$ `\boxminus` | $\div$ `\div`                       | $\odot$ `\odot`                     | $\unrhd$ `\unrhd`                     |
| $\boxplus$ `\boxplus`   | $\divideontimes$ `\divideontimes`   | $\ominus$ `\ominus`                 | $\uplus$ `\uplus`                     |
| $\boxtimes$ `\boxtimes` | $\dotplus$ `\dotplus`               | $\oplus$ `\oplus`                   | $\vee$ `\vee`                         |
| $\bullet$ `\bullet`     | $\doublebarwedge$ `\doublebarwedge` | $\otimes$ `\otimes`                 | $\veebar$ `\veebar`                   |
| $\Cap$ `\Cap`           | $\doublecap$ `\doublecap`           | $\oslash$ `\oslash`                 | $\wedge$ `\wedge`                     |
| $\cap$ `\cap`           | $\doublecup$ `\doublecup`           | $\pm$ `\pm` or `\plusmn`            | $\wr$ `\wr`                           |

* Direct Input: $+ - / * ⋅ ∘ ∙ ± × ÷ ∓ ∔ ∧ ∨ ∩ ∪ ≀ ⊎ ⊓ ⊔ ⊕ ⊖ ⊗ ⊘ ⊙ ⊚ ⊛ ⊝ ◯ ∖ {}$

### Fractions and Binomials

|                             |                               |                                                             |
| :-------------------------- | :---------------------------- | :---------------------------------------------------------- |
| $\frac{a}{b}$ `\frac{a}{b}` | $\tfrac{a}{b}$ `\tfrac{a}{b}` | $\genfrac ( ] {2pt}{1}a{a+1}$ `\genfrac ( ] {2pt}{1}a{a+1}` |
| ${a \over b}$ `{a \over b}` | $\dfrac{a}{b}$ `\dfrac{a}{b}` | ${a \above{2pt} b+1}$ `{a \above{2pt} b+1}`                 |
| $a/b$ `a/b`                 |                               | $\cfrac{a}{1 + \cfrac{1}{b}}$ `\cfrac{a}{1 + \cfrac{1}{b}}` |

|                                 |                                 |                             |
| :------------------------------ | :------------------------------ | :-------------------------- |
| $\binom{n}{k}$ `\binom{n}{k}`   | $\dbinom{n}{k}$ `\dbinom{n}{k}` | ${n\brace k}$ `{n\brace k}` |
| ${n \choose k}$ `{n \choose k}` | $\tbinom{n}{k}$ `\tbinom{n}{k}` | ${n\brack k}$ `{n\brack k}` |

### Math Operators

|                                         |                                                           |                       |                             |
| :-------------------------------------- | :-------------------------------------------------------- | :-------------------- | :-------------------------- |
| $\arcsin$ `\arcsin`                     | $\cosec$ `\cosec`                                         | $\deg$ `\deg`         | $\sec$ `\sec`               |
| $\arccos$ `\arccos`                     | $\cosh$ `\cosh`                                           | $\dim$ `\dim`         | $\sin$ `\sin`               |
| $\arctan$ `\arctan`                     | $\cot$ `\cot`                                             | $\exp$ `\exp`         | $\sinh$ `\sinh`             |
| $\arctg$ `\arctg`                       | $\cotg$ `\cotg`                                           | $\hom$ `\hom`         | $\sh$ `\sh`                 |
| $\arcctg$ `\arcctg`                     | $\coth$ `\coth`                                           | $\ker$ `\ker`         | $\tan$ `\tan`               |
| $\arg$ `\arg`                           | $\csc$ `\csc`                                             | $\lg$ `\lg`           | $\tanh$ `\tanh`             |
| $\ch$ `\ch`                             | $\ctg$ `\ctg`                                             | $\ln$ `\ln`           | $\tg$ `\tg`                 |
| $\cos$ `\cos`                           | $\cth$ `\cth`                                             | $\log$ `\log`         | $\th$ `\th`                 |
| $\operatorname{f}$ `\operatorname{f}`   |                                                           |                       |                             |
| $\argmax$ `\argmax`                     | $\injlim$ `\injlim`                                       | $\min$ `\min`         | $\varinjlim$ `\varinjlim`   |
| $\argmin$ `\argmin`                     | $\lim$ `\lim`                                             | $\plim$ `\plim`       | $\varliminf$ `\varliminf`   |
| $\det$ `\det`                           | $\liminf$ `\liminf`                                       | $\Pr$ `\Pr`           | $\varlimsup$ `\varlimsup`   |
| $\gcd$ `\gcd`                           | $\limsup$ `\limsup`                                       | $\projlim$ `\projlim` | $\varprojlim$ `\varprojlim` |
| $\inf$ `\inf`                           | $\max$ `\max`                                             | $\sup$ `\sup`         |                             |
| $\operatorname*{f}$ `\operatorname*{f}` | $\operatornamewithlimits{f}$ `\operatornamewithlimits{f}` |                       |                             |

* Functions in the bottom six rows of this table can take `\limits`.

### `\sqrt`

* $\sqrt{x}$ `\sqrt{x}`
* $\sqrt[3]{x}$ `\sqrt[3]{x}`

## Relations

* $\stackrel{!}{=}$ `\stackrel{!}{=}`

|                                                      |                                                |                                   |                                         |
| :--------------------------------------------------- | :--------------------------------------------- | :-------------------------------- | :-------------------------------------- |
| $=$ `=`                                              | $\doteqdot$ `\doteqdot`                        | $\lessapprox$ `\lessapprox`       | $\smile$ `\smile`                       |
| $<$ `<`                                              | $\eqcirc$ `\eqcirc`                            | $\lesseqgtr$ `\lesseqgtr`         | $\sqsubset$ `\sqsubset`                 |
| $>$ `>`                                              | $\eqcolon$ `\eqcolon` or `\minuscolon`         | $\lesseqqgtr$ `\lesseqqgtr`       | $\sqsubseteq$ `\sqsubseteq`             |
| $:$ `:`                                              | $\Eqcolon$ `\Eqcolon` or `\minuscoloncolon`    | $\lessgtr$ `\lessgtr`             | $\sqsupset$ `\sqsupset`                 |
| $\approx$ `\approx`                                  | $\eqqcolon$ `\eqqcolon` or `\equalscolon`      | $\lesssim$ `\lesssim`             | $\sqsupseteq$ `\sqsupseteq`             |
| $\approxcolon$ `\approxcolon`                        | $\Eqqcolon$ `\Eqqcolon` or `\equalscoloncolon` | $\ll$ `\ll`                       | $\Subset$ `\Subset`                     |
| $\approxcoloncolon$ `\approxcoloncolon`              | $\eqsim$ `\eqsim`                              | $\lll$ `\lll`                     | $\subset$ `\subset` or `\sub`           |
| $\approxeq$ `\approxeq`                              | $\eqslantgtr$ `\eqslantgtr`                    | $\llless$ `\llless`               | $\subseteq$ `\subseteq` or `\sube`      |
| $\asymp$ `\asymp`                                    | $\eqslantless$ `\eqslantless`                  | $\lt$ `\lt`                       | $\subseteqq$ `\subseteqq`               |
| $\backepsilon$ `\backepsilon`                        | $\equiv$ `\equiv`                              | $\mid$ `\mid`                     | $\succ$ `\succ`                         |
| $\backsim$ `\backsim`                                | $\fallingdotseq$ `\fallingdotseq`              | $\models$ `\models`               | $\succapprox$ `\succapprox`             |
| $\backsimeq$ `\backsimeq`                            | $\frown$ `\frown`                              | $\multimap$ `\multimap`           | $\succcurlyeq$ `\succcurlyeq`           |
| $\between$ `\between`                                | $\ge$ `\ge`                                    | $\origof$ `\origof`               | $\succeq$ `\succeq`                     |
| $\bowtie$ `\bowtie`                                  | $\geq$ `\geq`                                  | $\owns$ `\owns`                   | $\succsim$ `\succsim`                   |
| $\bumpeq$ `\bumpeq`                                  | $\geqq$ `\geqq`                                | $\parallel$ `\parallel`           | $\Supset$ `\Supset`                     |
| $\Bumpeq$ `\Bumpeq`                                  | $\geqslant$ `\geqslant`                        | $\perp$ `\perp`                   | $\supset$ `\supset`                     |
| $\circeq$ `\circeq`                                  | $\gg$ `\gg`                                    | $\pitchfork$ `\pitchfork`         | $\supseteq$ `\supseteq` or `\supe`      |
| $\colonapprox$ `\colonapprox`                        | $\ggg$ `\ggg`                                  | $\prec$ `\prec`                   | $\supseteqq$ `\supseteqq`               |
| $\Colonapprox$ `\Colonapprox` or `\coloncolonapprox` | $\gggtr$ `\gggtr`                              | $\precapprox$ `\precapprox`       | $\thickapprox$ `\thickapprox`           |
| $\coloneq$ `\coloneq` or `\colonminus`               | $\gt$ `\gt`                                    | $\preccurlyeq$ `\preccurlyeq`     | $\thicksim$ `\thicksim`                 |
| $\Coloneq$ `\Coloneq` or `\coloncolonminus`          | $\gtrapprox$ `\gtrapprox`                      | $\preceq$ `\preceq`               | $\trianglelefteq$ `\trianglelefteq`     |
| $\coloneqq$ `\coloneqq` or `\colonequals`            | $\gtreqless$ `\gtreqless`                      | $\precsim$ `\precsim`             | $\triangleq$ `\triangleq`               |
| $\Coloneqq$ `\Coloneqq` or `\coloncolonequals`       | $\gtreqqless$ `\gtreqqless`                    | $\propto$ `\propto`               | $\trianglerighteq$ `\trianglerighteq`   |
| $\colonsim$ `\colonsim`                              | $\gtrless$ `\gtrless`                          | $\risingdotseq$ `\risingdotseq`   | $\varpropto$ `\varpropto`               |
| $\Colonsim$ `\Colonsim` or `\coloncolonsim`          | $\gtrsim$ `\gtrsim`                            | $\shortmid$ `\shortmid`           | $\vartriangle$ `\vartriangle`           |
| $\cong$ `\cong`                                      | $\imageof$ `\imageof`                          | $\shortparallel$ `\shortparallel` | $\vartriangleleft$ `\vartriangleleft`   |
| $\curlyeqprec$ `\curlyeqprec`                        | $\in$ `\in` or `\isin`                         | $\sim$ `\sim`                     | $\vartriangleright$ `\vartriangleright` |
| $\curlyeqsucc$ `\curlyeqsucc`                        | $\Join$ `\Join`                                | $\simcolon$ `\simcolon`           | $\vcentcolon$ `\vcentcolon` or `\ratio` |
| $\dashv$ `\dashv`                                    | $\le$ `\le`                                    | $\simcoloncolon$ `\simcoloncolon` | $\vdash$ `\vdash`                       |
| $\dblcolon$ `\dblcolon` or<br> `\coloncolon`         | $\leq$ `\leq`                                  | $\simeq$ `\simeq`                 | $\vDash$ `\vDash`                       |
| $\doteq$ `\doteq`                                    | $\leqq$ `\leqq`                                | $\smallfrown$ `\smallfrown`       | $\Vdash$ `\Vdash`                       |
| $\Doteq$ `\Doteq`                                    | $\leqslant$ `\leqslant`                        | $\smallsmile$ `\smallsmile`       | $\Vvdash$ `\Vvdash`                     |

* Direct Input: $= < > : ∈ ∋ ∝ ∼ ∽ ≂ ≃ ≅ ≈ ≊ ≍ ≎ ≏ ≐ ≑ ≒ ≓ ≖ ≗ ≜ ≡ ≤ ≥ ≦ ≧ ≫ ≬ ≳ ≷ ≺ ≻ ≼ ≽ ≾ ≿ ⊂ ⊃ ⊆ ⊇ ⊏ ⊐ ⊑ ⊒ ⊢ ⊣ ⊩ ⊪ ⊸ ⋈ ⋍ ⋐ ⋑ ⋔ ⋙ ⋛ ⋞ ⋟ ⌢ ⌣ ⩾ ⪆ ⪌ ⪕ ⪖ ⪯ ⪰ ⪷ ⪸ ⫅ ⫆ ≲ ⩽ ⪅ ≶ ⋚ ⪋ ⟂ ⊨ $ `≔ ≕ ⩴`

### Negated Relations

* $\not =$ `\not =`

|                           |                                     |                                         |                                   |
| ------------------------- | ----------------------------------- | --------------------------------------- | --------------------------------- |
| $\gnapprox$ `\gnapprox`   | $\ngeqslant$ `\ngeqslant`           | $\nsubseteq$ `\nsubseteq`               | $\precneqq$ `\precneqq`           |
| $\gneq$ `\gneq`           | $\ngtr$ `\ngtr`                     | $\nsubseteqq$ `\nsubseteqq`             | $\precnsim$ `\precnsim`           |
| $\gneqq$ `\gneqq`         | $\nleq$ `\nleq`                     | $\nsucc$ `\nsucc`                       | $\subsetneq$ `\subsetneq`         |
| $\gnsim$ `\gnsim`         | $\nleqq$ `\nleqq`                   | $\nsucceq$ `\nsucceq`                   | $\subsetneqq$ `\subsetneqq`       |
| $\gvertneqq$ `\gvertneqq` | $\nleqslant$ `\nleqslant`           | $\nsupseteq$ `\nsupseteq`               | $\succnapprox$ `\succnapprox`     |
| $\lnapprox$ `\lnapprox`   | $\nless$ `\nless`                   | $\nsupseteqq$ `\nsupseteqq`             | $\succneqq$ `\succneqq`           |
| $\lneq$ `\lneq`           | $\nmid$ `\nmid`                     | $\ntriangleleft$ `\ntriangleleft`       | $\succnsim$ `\succnsim`           |
| $\lneqq$ `\lneqq`         | $\notin$ `\notin`                   | $\ntrianglelefteq$ `\ntrianglelefteq`   | $\supsetneq$ `\supsetneq`         |
| $\lnsim$ `\lnsim`         | $\notni$ `\notni`                   | $\ntriangleright$ `\ntriangleright`     | $\supsetneqq$ `\supsetneqq`       |
| $\lvertneqq$ `\lvertneqq` | $\nparallel$ `\nparallel`           | $\ntrianglerighteq$ `\ntrianglerighteq` | $\varsubsetneq$ `\varsubsetneq`   |
| $\ncong$ `\ncong`         | $\nprec$ `\nprec`                   | $\nvdash$ `\nvdash`                     | $\varsubsetneqq$ `\varsubsetneqq` |
| $\ne$ `\ne`               | $\npreceq$ `\npreceq`               | $\nvDash$ `\nvDash`                     | $\varsupsetneq$ `\varsupsetneq`   |
| $\neq$ `\neq`             | $\nshortmid$ `\nshortmid`           | $\nVDash$ `\nVDash`                     | $\varsupsetneqq$ `\varsupsetneqq` |
| $\ngeq$ `\ngeq`           | $\nshortparallel$ `\nshortparallel` | $\nVdash$ `\nVdash`                     |
| $\ngeqq$ `\ngeqq`         | $\nsim$ `\nsim`                     | $\precnapprox$ `\precnapprox`           |

* Direct Input: $∉ ∌ ∤ ∦ ≁ ≆ ≠ ≨ ≩ ≮ ≯ ≰ ≱ ⊀ ⊁ ⊈ ⊉ ⊊ ⊋ ⊬ ⊭ ⊮ ⊯ ⋠ ⋡ ⋦ ⋧ ⋨ ⋩ ⋬ ⋭ ⪇ ⪈ ⪉ ⪊ ⪵ ⪶ ⪹ ⪺ ⫋ ⫌$

### Arrows

|                                         |                                               |                                           |
| :-------------------------------------- | :-------------------------------------------- | :---------------------------------------- |
| $\circlearrowleft$ `\circlearrowleft`   | $\leftharpoonup$ `\leftharpoonup`             | $\rArr$ `\rArr`                           |
| $\circlearrowright$ `\circlearrowright` | $\leftleftarrows$ `\leftleftarrows`           | $\rarr$ `\rarr`                           |
| $\curvearrowleft$ `\curvearrowleft`     | $\leftrightarrow$ `\leftrightarrow`           | $\restriction$ `\restriction`             |
| $\curvearrowright$ `\curvearrowright`   | $\Leftrightarrow$ `\Leftrightarrow`           | $\rightarrow$ `\rightarrow`               |
| $\Darr$ `\Darr`                         | $\leftrightarrows$ `\leftrightarrows`         | $\Rightarrow$ `\Rightarrow`               |
| $\dArr$ `\dArr`                         | $\leftrightharpoons$ `\leftrightharpoons`     | $\rightarrowtail$ `\rightarrowtail`       |
| $\darr$ `\darr`                         | $\leftrightsquigarrow$ `\leftrightsquigarrow` | $\rightharpoondown$ `\rightharpoondown`   |
| $\dashleftarrow$ `\dashleftarrow`       | $\Lleftarrow$ `\Lleftarrow`                   | $\rightharpoonup$ `\rightharpoonup`       |
| $\dashrightarrow$ `\dashrightarrow`     | $\longleftarrow$ `\longleftarrow`             | $\rightleftarrows$ `\rightleftarrows`     |
| $\downarrow$ `\downarrow`               | $\Longleftarrow$ `\Longleftarrow`             | $\rightleftharpoons$ `\rightleftharpoons` |
| $\Downarrow$ `\Downarrow`               | $\longleftrightarrow$ `\longleftrightarrow`   | $\rightrightarrows$ `\rightrightarrows`   |
| $\downdownarrows$ `\downdownarrows`     | $\Longleftrightarrow$ `\Longleftrightarrow`   | $\rightsquigarrow$ `\rightsquigarrow`     |
| $\downharpoonleft$ `\downharpoonleft`   | $\longmapsto$ `\longmapsto`                   | $\Rrightarrow$ `\Rrightarrow`             |
| $\downharpoonright$ `\downharpoonright` | $\longrightarrow$ `\longrightarrow`           | $\Rsh$ `\Rsh`                             |
| $\gets$ `\gets`                         | $\Longrightarrow$ `\Longrightarrow`           | $\searrow$ `\searrow`                     |
| $\Harr$ `\Harr`                         | $\looparrowleft$ `\looparrowleft`             | $\swarrow$ `\swarrow`                     |
| $\hArr$ `\hArr`                         | $\looparrowright$ `\looparrowright`           | $\to$ `\to`                               |
| $\harr$ `\harr`                         | $\Lrarr$ `\Lrarr`                             | $\twoheadleftarrow$ `\twoheadleftarrow`   |
| $\hookleftarrow$ `\hookleftarrow`       | $\lrArr$ `\lrArr`                             | $\twoheadrightarrow$ `\twoheadrightarrow` |
| $\hookrightarrow$ `\hookrightarrow`     | $\lrarr$ `\lrarr`                             | $\Uarr$ `\Uarr`                           |
| $\iff$ `\iff`                           | $\Lsh$ `\Lsh`                                 | $\uArr$ `\uArr`                           |
| $\impliedby$ `\impliedby`               | $\mapsto$ `\mapsto`                           | $\uarr$ `\uarr`                           |
| $\implies$ `\implies`                   | $\nearrow$ `\nearrow`                         | $\uparrow$ `\uparrow`                     |
| $\Larr$ `\Larr`                         | $\nleftarrow$ `\nleftarrow`                   | $\Uparrow$ `\Uparrow`                     |
| $\lArr$ `\lArr`                         | $\nLeftarrow$ `\nLeftarrow`                   | $\updownarrow$ `\updownarrow`             |
| $\larr$ `\larr`                         | $\nleftrightarrow$ `\nleftrightarrow`         | $\Updownarrow$ `\Updownarrow`             |
| $\leadsto$ `\leadsto`                   | $\nLeftrightarrow$ `\nLeftrightarrow`         | $\upharpoonleft$ `\upharpoonleft`         |
| $\leftarrow$ `\leftarrow`               | $\nrightarrow$ `\nrightarrow`                 | $\upharpoonright$ `\upharpoonright`       |
| $\Leftarrow$ `\Leftarrow`               | $\nRightarrow$ `\nRightarrow`                 | $\upuparrows$ `\upuparrows`               |
| $\leftarrowtail$ `\leftarrowtail`       | $\nwarrow$ `\nwarrow`                         |
| $\leftharpoondown$ `\leftharpoondown`   | $\Rarr$ `\Rarr`                               |

* Direct Input: $← ↑ → ↓ ↔ ↕ ↖ ↗ ↘ ↙ ↚ ↛ ↞ ↠ ↢ ↣ ↦ ↩ ↪ ↫ ↬ ↭ ↮ ↰ ↱↶ ↷ ↺ ↻ ↼ ↽ ↾ ↾ ↿ ⇀ ⇁ ⇂ ⇃ ⇄ ⇆ ⇇ ⇈ ⇉ ⇊ ⇋ ⇌⇍ ⇎ ⇏ ⇐ ⇑ ⇒ ⇓ ⇔ ⇕ ⇚ ⇛ ⇝ ⇠ ⇢ ⟵ ⟶ ⟷ ⟸ ⟹ ⟺ ⟼$ ↽

#### Extensible Arrows

|                                                       |                                                         |
| :---------------------------------------------------- | :------------------------------------------------------ |
| $\xleftarrow{abc}$ `\xleftarrow{abc}`                 | $\xrightarrow[under]{over}$ `\xrightarrow[under]{over}` |
| $\xLeftarrow{abc}$ `\xLeftarrow{abc}`                 | $\xRightarrow{abc}$ `\xRightarrow{abc}`                 |
| $\xleftrightarrow{abc}$ `\xleftrightarrow{abc}`       | $\xLeftrightarrow{abc}$ `\xLeftrightarrow{abc}`         |
| $\xhookleftarrow{abc}$ `\xhookleftarrow{abc}`         | $\xhookrightarrow{abc}$ `\xhookrightarrow{abc}`         |
| $\xtwoheadleftarrow{abc}$ `\xtwoheadleftarrow{abc}`   | $\xtwoheadrightarrow{abc}$ `\xtwoheadrightarrow{abc}`   |
| $\xleftharpoonup{abc}$ `\xleftharpoonup{abc}`         | $\xrightharpoonup{abc}$ `\xrightharpoonup{abc}`         |
| $\xleftharpoondown{abc}$ `\xleftharpoondown{abc}`     | $\xrightharpoondown{abc}$ `\xrightharpoondown{abc}`     |
| $\xleftrightharpoons{abc}$ `\xleftrightharpoons{abc}` | $\xrightleftharpoons{abc}$ `\xrightleftharpoons{abc}`   |
| $\xtofrom{abc}$ `\xtofrom{abc}`                       | $\xmapsto{abc}$ `\xmapsto{abc}`                         |
| $\xlongequal{abc}$ `\xlongequal{abc}`                 |                                                         |

* Extensible arrows all can take an optional argument in the same manner as `\xrightarrow[under]{over}`.

## Special Notation

### Bra-ket Notation

|                           |                           |                                                                                                 |
| :------------------------ | :------------------------ | :---------------------------------------------------------------------------------------------- |
| $\bra{\phi}$ `\bra{\phi}` | $\ket{\psi}$ `\ket{\psi}` | $\braket{\phi\VERT\psi}$ `\braket{\phi&#124;\psi}`                                              |
| $\Bra{\phi}$ `\Bra{\phi}` | $\Ket{\psi}$ `\Ket{\psi}` | $\Braket{ ϕ \VERT \frac{∂^2}{∂ t^2} \VERT ψ }$ `\Braket{ ϕ &#124; \frac{∂^2}{∂ t^2} &#124; ψ }` |

## Style, Color, Size, and Font

### Class Assignment

* `\mathbin` `\mathclose` `\mathinner` `\mathop` `\mathopen` `\mathord` `\mathpunct` `\mathrel`

### Color

* $\color{red} F=ma$  `\color{red} F=ma`
* Note that `\color` acts like a switch. Other color functions expect the content to be a function argument:

* $\textcolor{red}{F=ma}$ `\textcolor{red}{F=ma}`
* $\textcolor{#228B22}{F=ma}$ `\textcolor{#228B22}{F=ma}`
* $\colorbox{blue}{$F=ma$}$ `\colorbox{aqua}{$F=ma$}`
* $\fcolorbox{red}{blue}{$F=ma$}$ `\fcolorbox{red}{aqua}{$F=ma$}`

* Note that, as in LaTeX, `\colorbox` & `\fcolorbox` renders its third argument as text, so you may want to switch back to math mode with `$` as in the examples above.
* For color definition, KaTeX color functions will accept the standard HTML [predefined color names](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value#Color_keywords). They will also accept an RGB argument in CSS hexa­decimal style. The "#" is optional before a six-digit specification.

### Font

|                                       |                                      |                                   |
| :------------------------------------ | :----------------------------------- | :-------------------------------- |
| $\mathrm{Ab0}$ `\mathrm{Ab0}`         | $\mathbf{Ab0}$ `\mathbf{Ab0}`        | $\mathit{Ab0}$ `\mathit{Ab0}`     |
| $\mathnormal{Ab0}$ `\mathnormal{Ab0}` | $\textbf{Ab0}$ `\textbf{Ab0}`        | $\textit{Ab0}$ `\textit{Ab0}`     |
| $\textrm{Ab0}$ `\textrm{Ab0}`         | $\bf Ab0$ `\bf Ab0`                  | $\it Ab0$ `\it Ab0`               |
| $\rm Ab0$ `\rm Ab0`                   | $\bold{Ab0}$ `\bold{Ab0}`            | $\textup{Ab0}$ `\textup{Ab0}`     |
| $\textnormal{Ab0}$ `\textnormal{Ab0}` | $\boldsymbol{Ab0}$ `\boldsymbol{Ab}` | $\Bbb{AB}$ `\Bbb{AB}`             |
| $\text{Ab0}$ `\text{Ab0}`             | $\bm{Ab0}$ `\bm{Ab0}`                | $\mathbb{AB}$ `\mathbb{AB}`       |
| $\mathsf{Ab0}$ `\mathsf{Ab0}`         | $\textmd{Ab0}$ `\textmd{Ab0}`        | $\frak{Ab0}$ `\frak{Ab0}`         |
| $\textsf{Ab0}$ `\textsf{Ab0}`         | $\mathtt{Ab0}$ `\mathtt{Ab0}`        | $\mathfrak{Ab0}$ `\mathfrak{Ab0}` |
| $\sf Ab0$ `\sf Ab0`                   | $\texttt{Ab0}$ `\texttt{Ab0}`        | $\mathcal{AB0}$ `\mathcal{AB0}`   |
|                                       | $\tt Ab0$ `\tt Ab0`                  | $\cal AB0$ `\cal AB0`             |
|                                       |                                      | $\mathscr{AB}$ `\mathscr{AB}`     |

* One can stack font family, font weight, and font shape by using the `\textXX` versions of the font functions. So `\textsf{\textbf{H}}` will produce $\textsf{\textbf{H}}$. The other versions do not stack, e.g., `\mathsf{\mathbf{H}}` will produce $\mathsf{\mathbf{H}}$.
* In cases where KaTeX fonts do not have a bold glyph, `\pmb` can simulate one. For example, `\pmb{\mu}` renders as : $\pmb{\mu}$

### Size

|                         |                                       |
| :---------------------- | :------------------------------------ |
| $\Huge AB$ `\Huge AB`   | $\normalsize AB$ `\normalsize AB`     |
| $\huge AB$ `\huge AB`   | $\small AB$ `\small AB`               |
| $\LARGE AB$ `\LARGE AB` | $\footnotesize AB$ `\footnotesize AB` |
| $\Large AB$ `\Large AB` | $\scriptsize AB$ `\scriptsize AB`     |
| $\large AB$ `\large AB` | $\tiny AB$ `\tiny AB`                 |

### Style

|                                                                                                                         |
| :---------------------------------------------------------------------------------------------------------------------- |
| $\displaystyle\sum_{i=1}^n$ `\displaystyle\sum_{i=1}^n`                                                                 |
| $\textstyle\sum_{i=1}^n$ `\textstyle\sum_{i=1}^n`                                                                       |
| $\scriptstyle x$ `\scriptstyle x` &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(The size of a first sub/superscript) |
| $\scriptscriptstyle x$ `\scriptscriptstyle x` (The size of subsequent sub/superscripts)                                 |
| $\lim\limits_x$ `\lim\limits_x`                                                                                         |
| $\lim\nolimits_x$ `\lim\nolimits_x`                                                                                     |
| $\verb!x^2!$ `\verb!x^2!`                                                                                               |

* `\text{...}` will accept nested `$...$` fragments and render them in math mode.

## Symbols and Punctuation

|                                                         |                                               |                                                 |
| :------------------------------------------------------ | :-------------------------------------------- | :---------------------------------------------- |
| `% comment`                                             | $\dots$ `\dots`                               | $\KaTeX$ `\KaTeX`                               |
| $\%$ `\%`                                               | $\cdots$ `\cdots`                             | $\LaTeX$ `\LaTeX`                               |
| $\#$ `\#`                                               | $\ddots$ `\ddots`                             | $\TeX$ `\TeX`                                   |
| $\&$ `\&`                                               | $\ldots$ `\ldots`                             | $\nabla$ `\nabla`                               |
| $\_$ `\_`                                               | $\vdots$ `\vdots`                             | $\infty$ `\infty`                               |
| $\text{\textunderscore}$ `\text{\textunderscore}`       | $\dotsb$ `\dotsb`                             | $\infin$ `\infin`                               |
| $\text{--}$ `\text{--}`                                 | $\dotsc$ `\dotsc`                             | $\checkmark$ `\checkmark`                       |
| $\text{\textendash}$ `\text{\textendash}`               | $\dotsi$ `\dotsi`                             | $\dag$ `\dag`                                   |
| $\text{---}$ `\text{---}`                               | $\dotsm$ `\dotsm`                             | $\dagger$ `\dagger`                             |
| $\text{\textemdash}$ `\text{\textemdash}`               | $\dotso$ `\dotso`                             | $\text{\textdagger}$ `\text{\textdagger}`       |
| $\text{\textasciitilde}$ `\text{\textasciitilde}`       | $\sdot$ `\sdot`                               | $\ddag$ `\ddag`                                 |
| $\text{\textasciicircum}$ `\text{\textasciicircum}`     | $\mathellipsis$ `\mathellipsis`               | $\ddagger$ `\ddagger`                           |
| $`$ <code>`</code>                                      | $\text{\textellipsis}$ `\text{\textellipsis}` | $\text{\textdaggerdbl}$ `\text{\textdaggerdbl}` |
| $\text{\textquoteleft}$ `text{\textquoteleft}`          | $\Box$ `\Box`                                 | $\Dagger$ `\Dagger`                             |
| $\lq$ `\lq`                                             | $\square$ `\square`                           | $\angle$ `\angle`                               |
| $\text{\textquoteright}$ `\text{\textquoteright}`       | $\blacksquare$ `\blacksquare`                 | $\measuredangle$ `\measuredangle`               |
| $\rq$ `\rq`                                             | $\triangle$ `\triangle`                       | $\sphericalangle$ `\sphericalangle`             |
| $\text{\textquotedblleft}$ `\text{\textquotedblleft}`   | $\triangledown$ `\triangledown`               | $\top$ `\top`                                   |
| $"$ `"`                                                 | $\triangleleft$ `\triangleleft`               | $\bot$ `\bot`                                   |
| $\text{\textquotedblright}$ `\text{\textquotedblright}` | $\triangleright$ `\triangleright`             | $\$$ `\$`                                       |
| $\colon$ `\colon`                                       | $\bigtriangledown$ `\bigtriangledown`         | $\text{\textdollar}$ `\text{\textdollar}`       |
| $\backprime$ `\backprime`                               | $\bigtriangleup$ `\bigtriangleup`             | $\pounds$ `\pounds`                             |
| $\prime$ `\prime`                                       | $\blacktriangle$ `\blacktriangle`             | $\mathsterling$ `\mathsterling`                 |
| $\text{\textless}$ `\text{\textless}`                   | $\blacktriangledown$ `\blacktriangledown`     | $\text{\textsterling}$ `\text{\textsterling}`   |
| $\text{\textgreater}$ `\text{\textgreater}`             | $\blacktriangleleft$ `\blacktriangleleft`     | $\yen$ `\yen`                                   |
| $\text{\textbar}$ `\text{\textbar}`                     | $\blacktriangleright$ `\blacktriangleright`   | $\surd$ `\surd`                                 |
| $\text{\textbardbl}$ `\text{\textbardbl}`               | $\diamond$ `\diamond`                         | $\degree$ `\degree`                             |
| $\text{\textbraceleft}$ `\text{\textbraceleft}`         | $\Diamond$ `\Diamond`                         | $\text{\textdegree}$ `\text{\textdegree}`       |
| $\text{\textbraceright}$ `\text{\textbraceright}`       | $\lozenge$ `\lozenge`                         | $\mho$ `\mho`                                   |
| $\text{\textbackslash}$ `\text{\textbackslash}`         | $\blacklozenge$ `\blacklozenge`               | $\diagdown$ `\diagdown`                         |
| $\text{\P}$ `\text{\P}` or `\P`                         | $\star$ `\star`                               | $\diagup$ `\diagup`                             |
| $\text{\S}$ `\text{\S}` or `\S`                         | $\bigstar$ `\bigstar`                         | $\flat$ `\flat`                                 |
| $\text{\sect}$ `\text{\sect}`                           | $\clubsuit$ `\clubsuit`                       | $\natural$ `\natural`                           |
| $\copyright$ `\copyright`                               | $\clubs$ `\clubs`                             | $\sharp$ `\sharp`                               |
| $\circledR$ `\circledR`                                 | $\diamondsuit$ `\diamondsuit`                 | $\heartsuit$ `\heartsuit`                       |
| $\text{\textregistered}$ `\text{\textregistered}`       | $\diamonds$ `\diamonds`                       | $\hearts$ `\hearts`                             |
| $\circledS$ `\circledS`                                 | $\spadesuit$ `\spadesuit`                     | $\spades$ `\spades`                             |
| $\text{\textcircled a}$ `\text{\textcircled a}`         | $\maltese$ `\maltese`                         | $\minuso$ `\minuso`                             |

* Direct Input: § ¶ $ £ ¥ ∇ ∞ · ∠ ∡ ∢ ♠ ♡ ♢ ♣ ♭ ♮ ♯ ✓ …  ⋮  ⋯  ⋱  !$ ‼ ⦵
