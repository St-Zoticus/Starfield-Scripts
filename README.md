# Starfield Custom Console Scripts & Tweaks

A collection of custom console scripts and configuration files designed to tweak and alter gameplay behaviors in *Starfield*.

This repository includes custom batch (`.txt`) scripts located in a dedicated `scripts` directory, along with a pre-configured `StarfieldCustom.ini` that automatically executes a master patch script (`ZoticusPatch.txt`) every time the game starts.

---

## 📁 Repository Structure

```text
├── StarfieldCustom.ini     # Enables custom INI settings and auto-runs ZoticusPatch.txt on startup
├── ZoticusPatch.txt    # Master patch script executed automatically at launch
└── scripts/
    └── [additional scripts].txt
```

---

## 🛠️ Installation

Follow these steps to set up the scripts and configuration files correctly.

### Step 1: Install `StarfieldCustom.ini`

1. Navigate to your **Documents** folder for Starfield:
```text
%USERPROFILE%\Documents\My Games\Starfield\

```


2. Copy `StarfieldCustom.ini` from this repository into that folder.
* *Note:* If you already have a `StarfieldCustom.ini`, open both files in a text editor and copy the contents of this repository's INI file into your existing one.



### Step 2: Install the `scripts` Folder

1. Locate your **root Starfield installation directory** (where `Starfield.exe` is located):
* **Steam default:** `C:\Program Files (x86)\Steam\steamapps\common\Starfield\`
* **Xbox / PC Game Pass default:** `C:\XboxGames\Starfield\Content\`
2. Copy the `scripts` and `ZoticusPatch.txt` folder from this repository directly into your main Starfield directory so that its path looks like:
```text
Starfield\ZoticusPatch.txt
Starfield\scripts\

```

---

## 🚀 Usage

### Automatic Execution

Thanks to `StarfieldCustom.ini`, the master patch file **`ZoticusPatch.txt`** will automatically run via `sStartingConsoleCommand` every time you boot the game. No manual console input is required for startup fixes or default baseline tweaks included in that file.

### Manual Console Execution

To run any specific script on demand while playing:

1. Open the in-game developer console by pressing the tilde key (`~` or `@` depending on your keyboard layout).
2. Type the following command and press **Enter**:

```text
bat 'scripts\<script_name>'

```

#### Example:

To manually run any script inside the `scripts` directory:

```text
bat 'scripts\$SCRIPT_NAME'

```

---

## ⚠️ Notes & Compatibility

* Executing certain console commands may disable **Steam / Xbox Achievements**. If you want to retain achievement functionality, consider using an achievement enabler mod (such as *Starfield Script Extender* with an achievement plugin).
* When creating new script files in the `scripts` directory, ensure they are saved as plain text (`.txt`) with `ANSI` or `UTF-8` encoding and Windows line endings enabled in your editor of choice.
