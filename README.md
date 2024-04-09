
## Hola a todos! prueba esta config!

<a href="https://awesomewm.org/"><img alt="AwesomeWM Logo" height="150" align = "left" src="https://awesomewm.org/doc/api/images/AUTOGEN_wibox_logo_logo_and_name.svg"></a>

<b> Awesome Environment </b>

¡Saludos y bienvenido al "Entorno AwesomeWM"!

Dentro de estas páginas digitales, descubrirás mis meticulosamente elaborados archivos de configuración AwesomeWM-una colección personal perfeccionada a la perfección.

Tanto si has llegado en busca de archivos de configuración AwesomeWM como si buscas inspiración para tu viaje Linux Rice, estás en el lugar adecuado.

Siéntete absolutamente libre de tomar prestadas mis creaciones, pero te pido amablemente que recuerdes dar crédito a quien lo merece.

AwesomeWM hace honor a su nombre: el gestor de ventanas para X más formidable y profundamente personalizable. Aunque configurarlo puede exigir una buena parte de tu tiempo y dedicación, puedo decir con confianza que el resultado estético bien merece el esfuerzo.

Gracias por visitar y explorar mi github.

<!-- INFORMATION -->

## :snowflake: ‎ <samp>Informaciones!</samp>

Detalles sobre mi configuración:

- **OS:** [Arch Linux](https://archlinux.org)
- **WM:** [awesome](https://github.com/awesomeWM/awesome)
- **Terminal:** [wezterm](https://github.com/wez/wezterm)
- **Shell:** [zsh](https://www.zsh.org/)
- **Editor:** [neovim](https://github.com/neovim/neovim) / [vscode](https://github.com/microsoft/vscode)
- **Compositor:** [picom](https://github.com/yshui/picom)
- **Application Launcher:** [rofi](https://github.com/davatorium/rofi)
- **Music Player** [ncmpcpp](https://github.com/ncmpcpp/ncmpcpp)

AwesomeWM Modulos:

- **[bling](https://github.com/blingcorp/bling)**
  - Añade nuevos diseños, módulos y widgets que intentan centrarse principalmente en la gestión de ventanas.
- **[color](https://github.com/andOrlando/color)**
  - Api limpia y eficiente para la conversión de color en lua.
- **[layout-machi](https://github.com/xinhaoyuan/layout-machi)**
  - Maquetación manual para Awesome con un editor interactivo.
- **[UPower](https://github.com/Aire-One/awesome-battery_widget)**
  - Un widget de batería basado en UPowerGlib para Awesome WM.
    
Funciones principales:

- **Eye-catching Colorscheme**
- **MacOS like window decorations**
- **Dashboard Panel**
- **Info Center Panel**
- **Notification Center Panel**
- **Bottom Panel**
- **Word Clock Lockscreen**
- **Minimalist Exit Screen**
- **Music Player**
- **App Launcher**
- **Github Activity Previews**
- **Brightness / Volume OSDs**
- **LayoutList PopUP**
- **Battery Indicator**
- **Wifi Indicator**
- **Calendar Widget**
- **Weather Widget**
- **Quick Settings Widget**
- **Hardware Monitor Widget**
- **Animated Workspace Indicator**
- **Beautiful Naughty Notification**
- **Right-Click Main Menu**

<br>

> Este repositorio tiene una wiki. Puede consultarlo haciendo clic en  [here](https://github.com/fito422480/AwesomeWM-Dotfiles/wiki).

<!-- SETUP -->

## :wrench: ‎ <samp>Setup</samp>

> Esto es paso a paso cómo instalar en su sistema. Sólo [R.T.F.M](https://en.wikipedia.org/wiki/RTFM).

<details>
<summary><b>1. Instale las dependencias necesarias y active los servicios</b></summary>
<br>

:warning: ‎ **Estas instrucciones de instalación sólo se proporcionan para Arch Linux (y otras distribuciones basadas en Arch)**

Suponiendo que su _YAY Helper_ is [YAY](https://github.com/Jguer/yay).

> En primer lugar, debes instalar [git version of AwesomeWM](https://github.com/awesomeWM/awesome/).

```sh
yay -S awesome-git
```

> Instalar necesesarias dependencias

```sh
yay -Sy picom-git wezterm rofi acpi acpid acpi_call upower lxappearance-gtk3 \
jq inotify-tools polkit-gnome xdotool xclip gpick ffmpeg blueman redshift \
pipewire pipewire-alsa pipewire-pulse alsa-utils brightnessctl feh maim \
mpv mpd mpc mpdris2 python-mutagen ncmpcpp playerctl --needed
```

> Habilitar Servicios

```sh
systemctl --user enable mpd.service
systemctl --user start mpd.service
```

</details>

<details>
<summary><b>2. Instalar</b></summary>
<br>

> Clonar este repositorio

```sh
git clone --depth 1 --recurse-submodules https://github.com/fito422480/AwesomeWM-Dotfiles.git
cd AwesomeWM-Dotfiles && git submodule update --remote --merge
```

> Copiar config archivos

```sh
cp -r config/* ~/.config/
```

> Instale algunas fuentes (principalmente fuentes de iconos) para que el texto y los iconos se muestren correctamente.

Fuentes Necesarias:

- **Roboto** - [here](https://fonts.google.com/specimen/Roboto)
- **Material Design Icons** - [here](https://github.com/google/material-design-icons)
- **Icomoon** - [here](https://www.dropbox.com/s/hrkub2yo9iapljz/icomoon.zip?dl=0)



> Por último, ahora puedes iniciar sesión con AwesomeWM

En este punto ya has instalado tu sistema. :tada:

Salga de su sesión de escritorio actual e inicie sesión en AwesomeWM

</details>

<!-- MISCELLANEOUS -->

<!-- ## :four_leaf_clover: ‎ <samp>Miscellaneous</samp>

<details>
<summary><b>VSCode Theme</b></summary>
<br>

<a href="#--------">
   <img src="" alt="VSCode theme preview" width="500px">
</a>

:comet: ‎ <samp>Yoru VSCode</samp>

Setup:

1. Install required extension

   - [Customize UI](https://marketplace.visualstudio.com/items?itemName=iocave.customize-ui)
   - [Carbon Product Icons](https://marketplace.visualstudio.com/items?itemName=antfu.icons-carbon)

   note: You can use any themes, but some of the colors will be overwritten by mine

2. copy config file

   ```sh
   cp misc/themes/vscode/User/settings.json ~/.config/Code/User

   ```

</details>

<details>
<summary><b>Neovim Theme</b></summary>
<br>

<a href="#--------">
   <img src="" alt="neovim theme preview" width="500px">
</a>

:cyclone: ‎ <samp>Yoru Neovim</samp>

This is nvchad's port of my aesthetic theme named `yoru`

To get this theme you have to use [nvchad](https://github.com/NvChad/NvChad) as your neovim config, and then apply my theme.

</details>

<details>
<summary><b>GTK Theme</b></summary>
<br>

<a href="#--------">
   <img src="" width="500px">
</a>

:milky_way: ‎ <samp>Yoru gtk theme</samp>

Setup:

1. Copy the themes to the themes folders
   ```sh
   sudo cp -rf misc/themes/gtk/AwesomeWM-Dotfiles/* /usr/share/themes
   cp -rf misc/themes/gtk/AwesomeWM-Dotfiles-GTK4/* ~/.config/gtk-4.0
   ```
2. Add this line on `~/.config/gtk-3.0/settings.ini` for left controls
   ```sh
   gtk-decoration-layout=close,maximize,minimize:menu
   ```

To apply the theme use ~~[lxappearance](https://archlinux.org/packages/community/x86_64/lxappearance)~~ [lxappearance-gtk3](https://archlinux.org/packages/community/x86_64/lxappearance-gtk3)

</details>

<details>
<summary><b>Kvantum Theme</b></summary>
<br>

<a href="#--------">
   <img src="" width="500px">
</a>

:ringed_planet: ‎ <samp>Yoru Kvantum Theme</samp>

Setup:

1. Copy the theme to the `~/.themes/` folders

```sh
cp -rf misc/themes/kvantum ~/.themes/
```

2. To apply the theme use the Kvantum Theme Engine

3. Open **Kvantum** and click `Select a Kvantum theme folder` and locate the theme it should be on `~/.themes/kvantum/Yoru/` and select that folder

4. After that click `Install this theme`

5. Then click the `Change/Delete Theme` section there should be a combo box that says `Select a theme` pick **Yoru** then click `Use this theme`

6. Now you should have the theme enabled and installed

</details>

<details>
<summary><b>Firefox Theme</b></summary>
<br>

<a href="#--------">
   <img src="" alt="firefox theme preview" width="500px">
</a>

:snowman_with_snow: ‎ <samp>Yoru Firefox</samp>

Setup:

1. Go to `about:config` in Firefox.
2. Search for `toolkit.legacyUserProfileCustomizations.stylesheets` and set it to `true`.
3. move the contents from [`misc/themes/firefox`](misc/themes/firefox) to `$HOME/.mozilla/firefox/xxxxxxxx.default-release/chrome`.

</details>

<details>
<summary><b>Discord Theme</b></summary>
<br>

<a href="#--------">
   <img src="" width="500px">
</a>

:speech_balloon: ‎ <samp>Yoru Discord Theme</samp>

Setup:

- Powercord

  Copy the discord folder to the powercord themes folder

  ```sh
  cp -rf misc/themes/discord /PATH/TO/DIRECTORY/WHICH/POWERCORD/IS/INSTALLED/src/Powercord/themes/
  ```

- Betterdiscord

  Copy the discord css to the betterdiscord themes folder

  ```sh
  cp misc/themes/discord/Yoru.theme.css ~/.config/BetterDiscord/themes/
  ```

> :warning: Using 3rd Party Clients are against Discord Terms and Service

</details>

<details>
<summary><b>Telegram Theme</b></summary>
<br>

<a href="#--------">
   <img src="" width="500px">
</a>

:telephone_receiver: <samp>Yoru Telegram Theme</samp>

Setup:

- First Method

  1. Go to: https://t.me/addtheme/yoru

  2. Open the link with your Telegram client of choice

  3. Apply the theme

- Second Method

  1. Open Telegram go to `Settings>Chat Settings>3DotMenu>Create new theme>IMPORT EXISTING THEME`

  2. Locate the theme `misc/telegram/Yoru.tdesktop-theme`

> :warning: This theme will only work on **Telegram Desktop** this won't on `MacOS, Android, and iOS`

</details> 

<details>
<summary><b>Touchpad tap-to-click & natural (reverse) scrolling (<a href="https://wiki.archlinux.org/title/Libinput#Tapping_button_re-mapping">libinput</a>)</b></summary>
<br>

`/etc/X11/xorg.conf.d/30-touchpad.conf`

```cfg
Section "InputClass"
    Identifier "touchpad"
    Driver "libinput"
    MatchIsTouchpad "on"
    Option "Tapping" "on"
    Option "TappingButtonMap" "lmr"
    Option "NaturalScrolling" "true"
EndSection
```

</details> -->

<!-- Yoru Colorscheme -->


