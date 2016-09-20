# task-shutdown-windows-script

Отключение компьютера под Windows по расписанию (20:00)

(для пользователя с правами "Администратор").
Нажатие: 

`  Win + R  `

Ввести компаду: 

`  cmd  `

Для обычного пользователя:

Поиск в меню пуск  

`  cmd  `

Запуск с правами администратора.

Код:

`schtasks /create /TN Shutdown /RL Highest /RU "System" /SC Daily /ST 20:00 /TR "%windir%\system32\shutdown.exe /s /t 60 /c \"Пора спать!!! \""
`

