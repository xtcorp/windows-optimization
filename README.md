![Windows Section](https://github.com/xtcorp/windows-optimization/blob/main/images/WindowsOptimization.png)

## 1. Отключаем Защитник
- Безопасность Windows -> Защита от вирусов и угроз -> Управление настройками
- Отключаем защиту в реальном времени

## 2. Отключаем Hyper-V + VBS
- Запускаем командную строку (cmd) от имени администратора
- ```bcdedit /set hypervisorlaunchtype off```
- Дожидаемся "Ok"

## 3. Удаляем Защитник + Mitigations
- [Скачать .exe](https://github.com/ionuttbara/windows-defender-remover/releases/)
- Запускаем от имени администратора
- Выбираем первый пункт, нажимая Y
- Ждем и программа сама поставит вас на перезагрузку

## 4. WinUtil
- Запускаем PowerShell от имени администратора
- ```irm https://christitus.com/win | iex```
- При первом запуске может попросить установить Chocolatey, соглашаемся
- После запуска WinUtil, переходим на вторую вкладку **Tweaks**
- Выбираем **Standard**
- Нажимаем **Run Tweaks** и смотрим в окно PowerShell, иногда нажимая Enter внутри него, так как может застрять
- Дожидаемся "Tweaks Are Finished"
- На этой же странице нажимаем **Add and Activate Ultimate Performance Profile**

## 5. Проверяем/выставляем профиль энергопотребления
- Панель управления -> Система и безопасность -> Параметры питания
- Выбираем профиль **Максимальная производительность**(Ultimate Performance), если он не выбран

## 6. Отключаем Bitlocker
- Если у вас компьютер Copilot+ сертификации, то не забудьте проверить Bitlocker и отключить его на всех дисках.
