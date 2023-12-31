# rEFInd theme Regular Minimalism #

For your convenience, the information is in two languages:  
Для вашего удобства информация изложена на двух языках:  
[In English](#In_English)  
[На Русском](#На_Русском)  

  
## <a name="In_English"></a> In English ##  

**rEFInd theme Regular Minimalism** - this is a simplified clean and minimalistic theme for the boot menu [rEFInd](https://www.rodsbooks.com/refind/index.html).

I created my own fork of theme [refind-theme-regular](https://github.com/bobafetthotmail/refind-theme-regular) from [bobafetthotmail](https://github.com/bobafetthotmail), which in turn is a fork that continues the abandoned theme [refind-theme-regular](https://github.com/munlik/refind-theme-regular) from [munlik](https://github.com/munlik).

Screenshot [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism) with OS **Windows 11** and OS **ElementaryOS** installed:
![Screenshot of the rEFInd boot menu with the refind-theme-regular-minimalism theme set](https://raw.github.com/Gutleibmann/refind-theme-regular-minimalism/master/refind-theme-regular-minimalism-screenshot.png)

The main changes made to the [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism) are described below.

## 1. Differences [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism) from [refind-theme-regular](https://github.com/bobafetthotmail/refind-theme-regular) ##
* Replaced the boot icon OS **Windows 11** from monotone to color in the **128х48** icon set.  
* The background of the dark theme has been changed from gray to black (This corrects the **"black square"** effect of the trobber when loading OS **Windows 11**).  
* The background of the download selector has been changed from black to gray (black to black, unfortunately, is not visible :D).  


## 2. Configuration settings of the predefined configuration file refind.conf of the boot menu [rEFInd](https://www.rodsbooks.com/refind/index.html) ##
* The OS selection timeout is set for 30 seconds.
* The option **Turn off after timeout** is enabled.
* The user interface options are disabled:
  * **Single User**: Submenu Options to Boot OS **macOS** in **Single User Mode**
  * **Tips**: Summary of commands in the rEFInd loader menu
  * **Arrows**: Selector arrows in the OS selection line
  * **Description**: Text note of the selected OS boot option in the rEFInd loader menu
  * **Icons**: device type icons for boot options
* The graphical boot option is enabled for OS **Windows 1x** and **UNIX**-based OS.
* Disabled **ALL** tools in the toolbox (Goodbye Swiss Knife).
* Search for bootloaders on **internal**, **external** and **optical** media is enabled.
* Automatic search for bootloaders in directories is disabled:
  * /boot/efi/EFI/boot
  * /boot/efi/EFI/Dell
  * /boot/efi/EFI/memtest86
  * /boot/efi/EFI/ubuntu
  * /boot/efi/EFI/BOOT
* File search disabled:
  * shim.efi
  * MokManager.efi
* Enabled theme [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism).

## 3. Instructions for installing and activating theme [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism)
**Note:** Further actions mean that everything is doing on a **UNIX**-based OS and **at least** you done installation of OS **Windows 11**, **UNIX**-based OS, boot menu [rEFInd](https://www.rodsbooks.com/refind/index.html).

* Cloning the theme repository [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism) to the user's **$HOME** directory:
   ```
   git clone https://github.com/gutleibmann/refind-theme-regular-minimalism.git
   ```
* Delete unnecessary files in a cloned repository:
   ```
   sudo rm -rf refind-theme-regular-minimalism/{.git,.gitkeep}
   ```
* Create the directory **themes** in the home directory of the boot menu [rEFInd](https://www.rodsbooks.com/refind/index.html):
   ```
   sudo mkdir -p /boot/efi/EFI/refind/themes
   ```
* Copy the cloned theme [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism) to the **themes** directory, created in **3.3.**:
   ```
   sudo cp -r refind-theme-regular-minimalism /boot/efi/EFI/refind/themes/
   ```
* Backup the existing configuration file **refind.conf** boot menu [rEFInd](https://www.rodsbooks.com/refind/index.html):
   ```
   sudo mv /boot/efi/EFI/refind/refind.conf /boot/efi/EFI/refind/refind.conf.backup
   ```
* Transfer the predefined **refind.conf** configuration file to the boot menu directory [rEFInd](https://www.rodsbooks.com/refind/index.html):
   ```
   sudo mv /boot/efi/EFI/refind/themes/refind-themes-regular-minimalism/refind.conf /boot/efi/EFI/refind/refind.conf
   ```

**P.S.:** If you want to use a set of icons other than **128х48**, then you need to do the actions described in paragraph **1.** for the set of icons you selected. It is recommended to use the software **Inkscape** to edit images.
If at any of the stages you encounter problems - write to me, I will try to help :)  
  
**P.S. for OS ElementaryOS users:** To correctly display OS **ElementaryOS** icon, you must remove or change the name of the default icon **VolumeIcon.png**, located in the root directory of the OS file system.  
**_____________**  
Best regards,  
Gutleibmann.
  
_____________



## <a name="На_Русском"></a> На Русском ## 

**rEFInd theme Regular Minimalism** - это упрощённая чистая и минималистичная тема для загрузочного меню [rEFInd](https://www.rodsbooks.com/refind/index.html).

Я создал собственную ветку темы [refind-theme-regular](https://github.com/bobafetthotmail/refind-theme-regular) от [bobafetthotmail](https://github.com/bobafetthotmail), которая в свою очередь является веткой продолжателем заброшенной темы [refind-theme-regular](https://github.com/munlik/refind-theme-regular) от [munlik](https://github.com/munlik).

Скриншот [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism) с установленными ОС **Windows 11** и ОС **ElementaryOS**:
![Скриншот загрузочного меню rEFInd с установленной темой refind-theme-regular-minimalism](https://raw.github.com/Gutleibmann/refind-theme-regular-minimalism/master/refind-theme-regular-minimalism-screenshot.png)

Ниже описаны основные изменения, внесенные в ветке [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism).

## 1. Отличия [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism) от [refind-theme-regular](https://github.com/bobafetthotmail/refind-theme-regular)
* Заменена иконка загрузки **Windows 11** с однотонной на цветную в пакете иконок **128-48**.
* Изменён фон тёмной темы с серого на чёрный (Тем самым исправляется эффект **"чёрного квадрата"** троббера при загрузке **Windows 11**).
* Изменён фон селектора загрузки с чёрного на серый (Чёрный на чёрном, к сожалению, не видно :D).

## 2. Настройки преднастроенного файла конфигурации refind.conf загрузочного меню [rEFInd](https://www.rodsbooks.com/refind/index.html)
* Таймаут выбора ОС выставлен на 30 секунд.
* Включена опция **Выключить после таймаута**.
* Отключены опции пользовательского интерфейса: 
  * **Один пользователь**: Параметры подменю для загрузки macOS в однопользовательском режиме
  * **Подсказки**: Краткая сводка по командам в меню загрузчика rEFInd
  * **Стрелки**: Стрелки-селекторы в строке выбора ОС
  * **Описание**: Текстовая заметка опции загрузки выбранной ОС в меню загрузчика rEFInd
  * **Значки**: Значки типа устройства для опций загрузки
* Включена опция загрузки в графическом режиме для ОС **Windows** и **UNIX**-подобных ОС.
* Отключены **ВСЕ** инструменты в строке инструментов (Прощай швейцарский нож).
* Включен поиск загрузчиков на **внутренних**, **внешних** и **оптических** носителях.
* Отключен автоматический поиск загрузчиков в директориях:
  * /boot/efi/EFI/boot
  * /boot/efi/EFI/Dell
  * /boot/efi/EFI/memtest86
  * /boot/efi/EFI/ubuntu
  * /boot/efi/EFI/BOOT
* Отключен поиск файлов:
  * shim.efi
  * MokManager.efi
* Включена тема [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism).

## 3. Инструкция по установке и активации темы [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism)
**Примечание:** Дальнейшие действия подразумевают, что всё выполняется в **UNIX**-подобной ОС и предварительно корректно установлены, как минимум, ОС **Windows 10**, **UNIX**-подобная ОС, загрузочное меню [rEFInd](https://www.rodsbooks.com/refind/index.html).

* Клонируем репозиторий темы [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism) в домашнюю директорию пользователя:
   ```
   git clone https://github.com/gutleibmann/refind-theme-regular-minimalism.git
   ```
* Удаляем лишние файлы в склонированном репозитории:
   ```
   sudo rm -rf refind-theme-regular-minimalism/{src,.git,.gitkeep}
   ```
* Создаём директорию **themes** в домашней директории загрузочного меню [rEFInd](https://www.rodsbooks.com/refind/index.html):
   ```
   sudo mkdir -p /boot/efi/EFI/refind/themes
   ```
* Копируем клонированный репозиторий темы [refind-theme-regular-minimalism](https://github.com/Gutleibmann/refind-theme-regular-minimalism) в директорию **themes**, созданную в **п. 3.3.**:
   ```
   sudo cp -r refind-theme-regular-minimalism /boot/efi/EFI/refind/themes/
   ```
* Создаём резервную копию существующего конфигурационного файла **refind.conf** загрузочного меню [rEFInd](https://www.rodsbooks.com/refind/index.html):
   ```
   sudo mv /boot/efi/EFI/refind/refind.conf /boot/efi/EFI/refind/refind.conf.backup
   ```
* Переносим преднастроенный конфигурационный файл **refind.conf** в директорию загрузочного меню [rEFInd](https://www.rodsbooks.com/refind/index.html):
   ```
   sudo mv /boot/efi/EFI/refind/themes/refind-themes-regular-minimalism/refind.conf /boot/efi/EFI/refind/refind.conf
   ```

**P.S.:** Если вы хотите использовать набор иконок отличный от **128х48**, то вам необходимо проделать действия описанные в **п. 1.** для выбранного вами набора иконок. Для редактирования изображений рекомендуется использовать ПО **Inkscape**.  
Если на каком-то из этапов вы столкнётесь с проблемами - пишите мне, постараюсь помочь :)  

**P.S. для пользователей ОС ElementaryOS:** Для корректного отображения иконки ОС **ElementaryOS** необходимо удалить или изменить название стандартной иконки **VolumeIcon.png**, расположенной в корневой директории файловой системы ОС.  
**_________________________________**  
С наилучшими пожеланиями,  
Gutleibmann.
