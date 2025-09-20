# cavvoh-unistore
A Universal-Updater DB where I will store my stuff for the 3DS family

## Installation
Please scan the next QR Code with the Universal Updater app:

![QR Code](https://github.com/Cavvoh/cavvoh-unistore/raw/main/qr-code.png)

## Building Atlas *.t3x.

<details><summary> Click to show/hide build instructions </summary>

<br>

- Download [DevKitPro](https://github.com/devkitPro/installer/releases/latest)
- Add directories `.\devkitPro\tools\bin`, and `.\devkitPro\msys2\usr\bin` to your Account PATH.
- You may also need to add the following directories to your Account PATH: `.\devkitPro\devkitARM\bin` and `.\devkitPro\libctru\include` 
- Start Powershell, and run the command `pacman -S tex3ds`.
- Create a new directory, and get textures you may need (48x48 size for icons).
- Create a file inside of your 'new' directory called `.\file.t3s`, then open it in a text editor and write the following strings to it:
```
--atlas -f rgba -z auto

{yourIconFile0.png}
{yourIconFile1.png}
{yourIconFile2.png}
{yourIconFile3.png}
```
`{yourIconFileX.png} is your PNG Icons in the Current Directory with the 'file.t3s' file`.

- After getting the icon images, you can now execute the command in the same directory using PowerShell.
- Type `tex3ds -i file.t3s -o cavvoh.t3x`
- It should generate a file with the Extension `*.t3x`, not `*.t3s`.
- That is your icon atlas.

</details>