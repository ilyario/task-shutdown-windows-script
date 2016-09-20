# task-shutdown-windows-script

Отключение компьютера под Windows по расписанию (20:00)

Нажатие: 

`  Win + R  `

Ввести компаду: 

`  cmd  `

Код:

`schtasks /create /TN Shutdown /RL Highest /RU "System" /SC Daily /ST 20:00 /TR "%windir%\system32\shutdown.exe /s /t 60 /c \"Пора спать!!! \""
`

