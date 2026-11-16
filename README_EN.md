
<div align="center">

# ⚡ SkPep

### Download. Install. Reload.

[🇵🇱 Polski](README_PL.md) • [🇬🇧 English](README_EN.md)

**A lightweight GitHub Skript downloader for Minecraft servers.**

</div>

---

## ✨ Features

- 📥 **GitHub Downloader** — Download `.sk` files directly from GitHub.
- 🔗 **Custom URLs** — Download scripts using direct GitHub Raw links.
- 📂 **Automatic Installation** — Files are saved in the `downloaded` directory.
- 🔄 **Automatic Reload** — Reload downloaded scripts automatically.
- 🏷️ **Custom Filenames** — Choose your own filename.
- 🛡️ **URL Validation** — Only `raw.githubusercontent.com` URLs are accepted.
- 🎨 **Colored Messages** — Clear and colorful console and in-game messages.

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
2. Place the `.jar` files inside your server's `plugins` directory.
3. Download `SkPep.sk`.
4. Put it inside `plugins/Skript/scripts/`.
5. Run:

```text
/sk reload SkPep.sk
```

## ⚙️ Configuration

```vb
options:
    prefix: §f[§bSkPep§f]
    repo: https://raw.githubusercontent.com/Pindoza/SkPep/main/scripts/
```

## 💻 Commands

| Command | Description |
|---|---|
| `/pep <name>` | Downloads a script from the repository |
| `/pep <name>.sk` | Downloads a script with its extension |
| `/pep link <URL>` | Downloads from a direct URL |
| `/pep link <URL> <name>` | Downloads using a custom filename |
| `/pepreload` | Reloads SkPep |

### Examples

```text
/pep example
/pep example.sk
/pep link https://raw.githubusercontent.com/Pindoza/SkPep/main/scripts/example.sk
/pep link https://raw.githubusercontent.com/Pindoza/SkPep/main/scripts/example.sk custom
```

## 📁 Repository Structure

```text
SkPep/
├── README.md
├── README_PL.md
├── README_EN.md
├── SkPep.sk
└── scripts/
    ├── example.sk
    ├── another-script.sk
    └── my-script.sk
```

## 📚 Available Scripts

All publicly downloadable scripts are stored in:

`/scripts/`

To add a new script:

1. Place your `.sk` file inside the `scripts/` directory.
2. Push your changes to GitHub.
3. Download it on your server using `/pep <name>`.

## 📂 Download Location

```text
plugins/Skript/scripts/downloaded/
```

## 🔐 Permissions

| Permission | Description |
|---|---|
| `skpep.use` | Access to SkPep commands |

## ⚠️ Security

- Only download scripts from trusted sources.
- Skript files can execute server-side code.
- Review scripts before installing them.
- Avoid installing unknown scripts on production servers.

---

<div align="center">

**⚡ SkPep — Download. Install. Reload.**

</div>
