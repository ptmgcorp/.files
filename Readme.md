# Starship Terminal
### Installation
<details>
<summary>Linux</summary>

Install the latest version for your system:
```sh
curl -sS https://starship.rs/install.sh | sh
```
### Step 2. Set up your shell to use Starship
Add the following to the end of `~/.bashrc`:
```sh
eval "$(starship init bash)"
```
</details>

<details>
<summary>macOS</summary>
  
Install the latest version for your system:
```sh
curl -sS https://starship.rs/install.sh | sh
```
### Step 2. Set up your shell to use Starship
Add the following to the end of `~/.bashrc`:

```sh
eval "$(starship init bash)"
```
</details>

<details>
<summary>Windows</summary>
  
Install the latest version for your system with the MSI-installers from the [releases section](https://github.com/starship/starship/releases/latest).
Install Starship using any of the following package managers:
| Repository      | Instructions                            |
| --------------- | --------------------------------------- |
| [winget]        | `winget install --id Starship.Starship` |

### Step 2. Set up your shell to use Starship
<details>
<summary>Cmd</summary>

You need to use [Clink](https://chrisant996.github.io/clink/clink.html) (v1.2.30+) with Cmd.
Create a file at this path `%LocalAppData%\clink\starship.lua` with the following contents:

```lua
load(io.popen('starship init cmd'):read("*a"))()
```

</details>
<details>
<summary>PowerShell</summary>

Add the following to the end of your PowerShell configuration (find it by running `$PROFILE`):

```powershell
Invoke-Expression (&starship init powershell)
```

</details>

</details>

### Configuration
To get started configuring starship, create the following file: ~/.config/starship.toml.
```
mkdir -p ~/.config
wget https://raw.githubusercontent.com/ptmgcorp/.files/main/.config/starship.toml -P ~/.config/
```

#### Script to bat converter
```
https://daniel-sc.github.io/bash-shell-to-bat-converter/
```
