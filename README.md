
<div align="center">

# ⚡ SkPep

### Download. Install. Reload.

**A lightweight Skript downloader for Minecraft servers.**

[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.5-brightgreen?style=for-the-badge&logo=minecraft)](https://www.minecraft.net/)
[![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=openjdk)](https://www.java.com/)
[![Skript](https://img.shields.io/badge/Skript-2.17+-blue?style=for-the-badge)](https://github.com/SkriptLang/Skript)

**Download Skript files directly from GitHub and install them on your server.**

</div>

---

## ✨ Features

- 📥 **GitHub Downloader** — Download `.sk` files directly from GitHub.
- 🔗 **Custom URLs** — Download scripts using direct `raw.githubusercontent.com` links.
- 📂 **Automatic Installation** — Downloaded scripts are saved in the `downloaded` directory.
- 🔄 **Automatic Reload** — Reload downloaded scripts immediately after installation.
- 🏷️ **Custom Filenames** — Choose your own filename when downloading a script.
- 🛡️ **URL Validation** — Only direct GitHub Raw URLs are accepted by `/pep link`.
- 🎨 **Colored Console Messages** — Clear and colorful status messages.

## 📦 Requirements

| Dependency | Version |
|---|---|
| Minecraft | 1.21.5 |
| Java | 21+ |
| Skript | 2.17+ |
| skJson | 5.6.0 |
| skript-reflect | 2.6.2 |

## 📥 Installation

1. Download the required dependencies.
2. Put the addon JAR files into your server's `plugins` directory.
3. Download `SkPep.sk`.
4. Put `SkPep.sk` into:

   `plugins/Skript/scripts/`

5. Open `SkPep.sk` and configure the repository URL.
6. Reload Skript:

```text
/sk reload SkPep.sk
```

## ⚙️ Configuration

The repository URL determines where SkPep searches for scripts when using `/pep <name>`.

```vb
options:
    prefix: §f[§bSkPep§f]
    repo: https://raw.githubusercontent.com/Pindoza/SkPep/main/scripts/
```

The URL above points to the `scripts/` directory in this repository.

## 💻 Commands

### `/pep <name>`

Downloads a script from the configured GitHub repository.

```text
/pep example
/pep example.sk
```

### `/pep link <URL> [name]`

Downloads a script using a direct GitHub Raw URL.

```text
/pep link https://raw.githubusercontent.com/Pindoza/SkPep/main/scripts/example.sk
```

You can also specify a custom filename:

```text
/pep link https://raw.githubusercontent.com/Pindoza/SkPep/main/scripts/example.sk custom
```

### `/pepreload`

Reloads SkPep itself.

```text
/pepreload
```

## 📁 Repository Structure

```text
SkPep/
│
├── README.md
├── SkPep.sk
│
└── scripts/
    ├── example.sk
    ├── another-script.sk
    └── my-script.sk
```

### 📚 Available Scripts

All downloadable scripts are stored in the `scripts/` directory.

To download a script, use its filename without the `.sk` extension:

```text
/pep example
```

To add a new downloadable script:

1. Upload your `.sk` file into the `scripts/` directory.
2. Commit and push your changes.
3. Use `/pep <filename>` on your server.

## 📂 Download Location

Downloaded scripts are stored locally in:

```text
plugins/Skript/scripts/downloaded/
```

SkPep creates the directory automatically when needed.

## 🔐 Permissions

| Permission | Description |
|---|---|
| `skpep.use` | Allows using SkPep commands |

## ⚠️ Security

- Only use scripts from sources you trust.
- Downloaded Skript files are executable server code.
- Check scripts before installing them on a production server.
- `/pep link` accepts URLs from `raw.githubusercontent.com`.

## 🛠️ Troubleshooting

**HTTP 404**

The requested file does not exist at the specified GitHub path. Check its filename and repository location.

**HTTP errors**

Check your server's internet connection and the Raw GitHub URL.

**Script failed to reload**

Check the Skript console for syntax errors in the downloaded file.

**Missing dependencies**

Make sure skJson and skript-reflect are installed and enabled.

---

<div align="center">

### ⚡ SkPep

**Made for Minecraft server administrators.**

⭐ If you find SkPep useful, consider giving the repository a star!

</div>
