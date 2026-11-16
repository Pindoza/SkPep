# SkRaid

A custom raid system for Minecraft servers, created using Skript.

SkRaid comes in two versions. Both provide the same raid system, but differ in how mob spawn locations are handled.

## 📦 Versions

### SkRaid-Sarea

**Manual spawn location configuration.**

- Requires manually configured mob spawn locations.
- Gives you control over where raid mobs spawn.
- Recommended if you want to choose specific spawn locations.

### SkRaid-NoSarea

**Automatic mob spawn locations.**

- Does not require manually configured spawn locations.
- Handles mob spawn locations automatically.
- Recommended if you don't want to configure spawn locations yourself.

## ⚠️ Important — Only One Version Allowed

**You can install only ONE SkRaid version at a time!**

- Do not install `SkRaid-Sarea` and `SkRaid-NoSarea` simultaneously.
- Both versions use the same raid system and may conflict with each other.
- Remove the other version before installing or enabling a different one.

Running both versions together may cause unexpected behavior, duplicate events or conflicts.

## ✨ Features

- Custom Minecraft raid system
- Two versions with different spawn location handling
- Skript-based implementation
- Designed for Minecraft servers

## 📋 Requirements

- Minecraft 1.21.5
- Java 21+
- Skript 2.17+

## 📥 Installation

1. Choose the version you want to use:
   - `SkRaid-Sarea`
   - `SkRaid-NoSarea`
2. Download the `.sk` file.
3. Place it inside your Skript scripts folder:

   `plugins/Skript/scripts/`

4. Make sure the other SkRaid version is not installed.
5. Reload Skript:

   `/sk reload <filename>`

## 🔄 Switching Versions

To switch between versions:

1. Disable or remove your current SkRaid script.
2. Install the other version.
3. Reload Skript.

**Never run both versions at the same time.**

## 📁 Versions Comparison

| Feature | SkRaid-Sarea | SkRaid-NoSarea |
|---|---|---|
| Manual spawn locations | Required | Not required |
| Automatic spawn locations | No | Yes |
| Same raid system | Yes | Yes |
| Can run together | No | No |

## 📄 License

See the repository for license information.
