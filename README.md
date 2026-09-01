
# LUNEX

### Modern & Customizable Backpack Loader for Roblox

LUNEX is a modern, lightweight, and customizable Backpack system for Roblox.

It is designed to provide a cleaner and more flexible alternative to the default Roblox Backpack, while keeping the installation and customization process simple for developers.

LUNEX uses a modular package structure, allowing the entire system to be moved between Roblox services without manually rebuilding its internal components.

---

## ✨ Features

- 🎒 Modern Backpack UI
- 🎨 Fully customizable appearance
- 🔤 Custom font support
- 📦 Configurable inventory slots
- 🔍 Built-in item search
- 🗂️ Item categories
- ❤️ Favorite item support
- ⚙️ Attribute-based configuration
- 🧩 Modular package structure
- 📁 Self-contained UI components and templates
- 🚀 Automatic Backpack initialization
- 🔄 Easy to move between Roblox services

---

# 📦 Installation

## 1. Insert the LUNEX Package

Place the entire LUNEX package inside your game.

The recommended setup is:

```text
StarterPlayer
└── StarterPlayerScripts
    └── Lunex
        └── Lunex (LocalScript)
            └── lunex (ModuleScript)
                ├── Packages
                ├── StrokeTemplate
                ├── Api
                ├── Favorite_Item
                ├── CategoryFrame
                ├── Fav
                └── CategoryTemplate
````

> **Important:** Keep the internal structure of the LUNEX package intact.
> The included components are required by the Backpack system.

---

## 2. Run Your Game

After placing the LUNEX package in your game, simply start the game.

LUNEX will initialize automatically and replace the default Roblox Backpack with the LUNEX interface.

No additional setup is required for the default configuration.

---

# 📁 Package Structure

The LUNEX package contains all components required by the Backpack system.

```text
Lunex
└── Lunex (LocalScript)
    └── lunex (ModuleScript)
        ├── Packages
        ├── StrokeTemplate
        ├── Api
        ├── Favorite_Item
        ├── CategoryFrame
        ├── Fav
        └── CategoryTemplate
```

### `Lunex`

The main **LocalScript** responsible for loading and initializing the LUNEX Backpack.

### `lunex`

The main LUNEX module containing the Backpack system and its configuration.

### `Packages`

Contains internal modules and dependencies used by LUNEX.

### `Api`

Provides internal API functionality used by the Backpack system.

### `CategoryFrame`

UI component used for displaying Backpack item categories.

### `CategoryTemplate`

Template used to generate category elements.

### `Favorite_Item`

Component responsible for favorite item functionality.

### `Fav`

UI element used for the favorite system.

### `StrokeTemplate`

Template used for UI stroke elements.

---

# 🎨 Customization

LUNEX is built with customization in mind.

You can change the appearance of the Backpack directly through **Attributes** on the `lunex` ModuleScript.

You do **not** need to modify the source code for common visual customization.

### Available Attributes

| Attribute                  | Description                            |
| -------------------------- | -------------------------------------- |
| `BackgroundColor`          | Main Backpack background color         |
| `BackgroundTransparency`   | Main Backpack transparency             |
| `BorderColor`              | Backpack border color                  |
| `CornerRadius`             | UI corner radius                       |
| `DraggableColor`           | Color of the draggable area            |
| `EquippedColor`            | Color used for equipped slots          |
| `FullSlots`                | Maximum number of full inventory slots |
| `LabelFont`                | Font used for item labels              |
| `MiniSlots`                | Number of minimized slots              |
| `SearchBoxColor`           | Search box color                       |
| `SearchBoxTransparency`    | Search box transparency                |
| `SlotEquipStrokeThickness` | Equipped slot stroke thickness         |
| `SlotFont`                 | Font used for inventory slot text      |

---

# ⚙️ Configuration

Select the `lunex` ModuleScript and configure its Attributes from the Roblox Properties panel.

For example:

```text
BackgroundColor        = [31, 31, 31]
BackgroundTransparency = 0.25
BorderColor            = [255, 255, 255]

CornerRadius           = 8

DraggableColor         = [48, 48, 48]
EquippedColor          = [90, 142, 233]

FullSlots              = 10
MiniSlots              = 3

SearchBoxColor         = [94, 94, 94]
SearchBoxTransparency  = 0.5

LabelFont              = Comic Neue Angular
SlotFont               = Comic Neue Angular
```

This allows you to create your own Backpack style without editing the LUNEX source code.

---

# 🔄 Moving LUNEX

LUNEX is packaged so that the entire system can be moved as a single package.

For example, you can move the LUNEX package from:

```text
StarterPlayer
└── StarterPlayerScripts
    └── Lunex
```

to another suitable location such as:

```text
ReplicatedStorage
└── Lunex
```

The internal structure should remain unchanged.

```text
Lunex
└── Lunex
    └── lunex
        ├── Packages
        ├── StrokeTemplate
        ├── Api
        ├── Favorite_Item
        ├── CategoryFrame
        ├── Fav
        └── CategoryTemplate
```

### Important

When moving LUNEX, always move the **entire package** instead of moving individual components.

This ensures that all required modules, templates, and UI dependencies remain together.

> **Tip:** If you are using the default LUNEX loader, `StarterPlayerScripts` is recommended because the Backpack is a client-side system.

---

# 🧩 Recommended Structure

For most Roblox games, we recommend:

```text
StarterPlayer
└── StarterPlayerScripts
    └── Lunex
        └── Lunex (LocalScript)
            └── lunex (ModuleScript)
                ├── Packages
                ├── StrokeTemplate
                ├── Api
                ├── Favorite_Item
                ├── CategoryFrame
                ├── Fav
                └── CategoryTemplate
```

This keeps the LUNEX system self-contained and easy to manage.

---

# 🚀 Why LUNEX?

The default Roblox Backpack provides the basic inventory functionality, but developers often need more control over its appearance and user experience.

LUNEX provides:

* A modern interface
* Easy customization
* Modular architecture
* Attribute-based configuration
* A clean and organized package
* Minimal setup
* Flexible integration into existing Roblox projects

Whether you want a simple Backpack or a completely customized inventory experience, LUNEX is designed to give you control without requiring extensive source-code modifications.

---

# 📄 License

Please see the repository license for information regarding usage, modification, and redistribution.

---

<div align="center">

### LUNEX

**Modern Backpack. Simple Integration. Full Customization.**

*A modern, customizable Backpack experience for Roblox.*

</div>
