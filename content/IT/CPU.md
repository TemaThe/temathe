[Степик Курс](https://stepik.org/lesson/41871/step/3?unit=20186)



CPU

CPU do only 3 things 
	1. Read from memory instruction + args
	2. Execute operation
	3. Put result to memory
	   
##### Классы инструкции для процессоров
	Инструкции копирования
		movq <src>, <dst> 
		
	Арифметические
		 addq <src>, <dst>
		sub
		incq /desq увеличить/уменьшить на 1
		mulq <op> умножение второй всегда RAX/RDX
		divq 128 бит
		
	Перехода
		Условного
		Безоусловного
	Прочие


Регистры 
это именнованная память (у каждного есть свое имя) 
размер 8/16/32/64 бит (макс опр разрядность процессора)
x86-64 16 штук (по 8 бит (макс опр разрядность процессора) int+16 float
ARM 64 32 float +32 float
 


Регистры общего назначения
Регистры спец назначения
	флаговый регистр
	Указатель команд - RIP(адресс след инстр)
	Флаговый (состояния проц ???)
	указатель стека RSP


	

#### Стек 
область памяти на который указывает регистр RSP
pushq<src>  положить
	уменьшает RSP на 8 и сохр по полученому адресу src
popq <dst> удаляет значение стека и сохр <dst>
			после увеличивает значение RSP на 8



Метка / Label имя некоторого адреса в памяти

Инструкция безусловного перехода
изм регистр RIP 
jmp<label>
call <label> 
retq - инстр перехода

Функция 
	можно вызвавать
	вернуть упр откуда вызвали




