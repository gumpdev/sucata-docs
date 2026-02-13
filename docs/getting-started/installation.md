# Installation

This guide explains how to install sucata on Windows, macOS, and Linux, or build
it from source.

## 📦 Installing Prebuilt Binaries

Install sucata with a prebuilt binary, without need to configure or install any
dependencies.

### 🪟 Windows

1. Open PowerShell.
2. Run the following command:

```powershell
irm https://raw.githubusercontent.com/gumpdev/sucata/refs/heads/main/install_windows.ps1 | iex
```

3. Restart your terminal.
4. Now you can use the command `sucata` in your terminal.

> **Warning** This command downloads and executes the official installation
> script. It will: Download sucata, Install it on your system and Add it to your
> system PATH

### 🐧 MacOs/Linux

1. Open your terminal.
2. Run the following command:

```bash
curl -fsSL https://raw.githubusercontent.com/gumpdev/sucata/refs/heads/main/install_unix.sh | sh
```

3. Restart your terminal.
4. Now you can use the command `sucata` in your terminal.

> **Warning** This command downloads and executes the official installation
> script. It will: Download sucata, Install it on your system and Add it to your
> system PATH

### 🛠 Building from Source

If you prefer to build sucata manually:

1. You need to install: Odin and C++ compiler (MSVC, Clang, or GCC)
2. [Clone the repository](https://github.com/gumpdev/sucata)
3. Go to the folder /sokol/ and
   [build the sokol binaries](https://github.com/floooh/sokol-odin/tree/main?tab=readme-ov-file#build)
4. You go to the repository root, then build the sucata binaries using:

```odin
odin build .
```

5. (optional) Add the binary to the path of your system
6. All done you now can use the sucata

## 🌙 Installing Lua Addon

You can install an sucata lua addon on the sumneko's lua extension for better
auto completion

1. Install [sumneko's lua extension](https://luals.github.io) in your favorite
   IDE
2. Open the [Addon Manager](https://luals.github.io/wiki/addons/#addon-manager)
3. Search for 'sucata' and install the sucata addon
