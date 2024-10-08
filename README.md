![Windows Section](https://github.com/xtcorp/windows-optimization/blob/main/images/WindowsOptimization.png)

## 1. Отключаем Защитник
- Безопасность Windows -> Защита от вирусов и угроз -> Управление настройками
- Отключаем все пункты

## 2. Удаление Defender
- [Скачать.](https://github.com/ionuttbara/windows-defender-remover/releases/)
- Запускаем от имени администратора
- Перезагружаемся

## 3. Отключаем изоляцию ядра
- Безопасность Windows -> Безопасность устройства
- Заходим в сведения под каждым пунктом и отключаем все возможное внутри

## 4. Отключаем Hyper-V
- Запускаем командную строку (cmd) от имени администратора
- ```bcdedit /set hypervisorlaunchtype off```
- Дожидаемся "Ok"

## 5. WinUtil
- Запускаем PowerShell от имени администратора
- ```irm https://christitus.com/win | iex```
- При первом запуске может попросить установить Chocolatey, соглашаемся
- После запуска WinUtil, переходим на вторую вкладку **Tweaks**
- Выбираем в Recommended Selections либо **Desktop**, если у вас стационарный компьютер, либо **Laptop**, если у вас ноутбук
- Нажимаем **Run Tweaks** и смотри в окно PowerShell, иногда нажимая Enter внутри него, так как может застрять
- Дожидаемся "Tweaks Are Finished"
- На этой же странице нажимаем **Add and Activate Ultimate Performance Profile**

## 6. Выставляем/проверяем профиль энергопотребления
- Панель управления -> Система и безопасность -> Параметры питания
- Выбираем профиль **Максимальная производительность**(Ultimate Performance)

## 7. Manage Speculative Execution Protection Settings
- [Скачать.](https://drive.google.com/file/d/1m3aLZGD3cA8pgSZvvnvZ8j-see9ipDRJ/view?usp=sharing)
- При первом запуске может попросить установить SpeculativeControl, соглашаемся, написав цифру **2** и нажав Enter
- Выбираем [9] Disable all Speculative Execution Protection Mitigations, написав цифру **9** и нажав Enter
- Выбираем [1] Disable now, написав цифру **1** и нажав Enter
- **(ВАЖНО!!)** Выбираем [1] Restart now, написав цифру **1** и нажав Enter

## 8. Отключаем Bitlocker
- Ждем 24H2 для этого пункта.
