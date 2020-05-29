# WinRAR-Keygen

## 1. What is WinRAR?

WinRAR is a trialware file archiver utility for Windows, developed by Eugene Roshal of win.rar GmbH. 

It can create and view archives in RAR or ZIP file formats and unpack numerous archive file formats. 

WinRAR is not a free software. If you want to use it, you should pay to [__RARLAB__](https://rarlab.com/) and then you will get a license file named `rarreg.key`. 

This repository will tell you how WinRAR license file `"rarreg.key"` is generated. 

## 2. How is "rarreg.key" generated?

See [here](README.HOW_DOES_IT_WORK.md).

## 3. How to build?

### 3.1 Prerequisites

1. Please make sure that you have __Visual Studio 2019__ or the higher. Because this is a VS2019 project.

2. Please make sure you have installed `vcpkg` and the following libraries: 

   * `mpir:x86-windows-static`
   * `mpir:x64-windows-static`

   is installed.

   You can install them by:

   ```console
   $ vcpkg install mpir:x86-windows-static
   $ vcpkg install mpir:x64-windows-static
   ```

3. Your `vcpkg` has been integrated into your __Visual Studio__, which means you have run 

   ```console
   $ vcpkg integrate install
   ```
   
   successfully.

### 3.2 Build

1. Open this project in __Visual Studio__.

2. Select `Release` configuration.

3. Select __Build > Build Solution__.

You will see executable files in `bin/` directory. 

## 4. How to Use?

```
Usage:
        winrar-keygen.exe <your name> <license type>

Example:

        winrar-keygen.exe "Prototype" "Unlimited Company License"
  or:
        winrar-keygen.exe "Prototype" "Unlimited Company License" > rarreg.key
```

```console
$ winrar-keygen.exe "Prototype" "Unlimited Company License"
RAR registration data
Prototype
Unlimited Company License
UID=4d07242e8f4863658c8c
64122122508c8cd2af98c0c8b88723e11464203164d4fcd57168ad
3bb428f168f7a8e98a89604c1960b1d7f798616191cdc1c16a611c
d94f48dd7749d20c64cee4e7afcaf5b31e8ffd1be082285cb5c1e8
abbf2c6387187f512a0d242a56b94b5ecc608508c3b89aef817de3
6023e3a0d1610eafdae4571ec42e68a325f125a09af5b31e8ffd1b
e082285cb491dd4899f59ec5194e7c90ff7d457366e0030760a95c
8f47a39954e36a787c7076b518111fa29f219127641c1958429930
```

### Credits: z9421371