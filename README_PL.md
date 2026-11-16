
<div align="center">

# ⚡ SkPep

### Pobieraj. Instaluj. Przeładowuj.

[🇵🇱 Polski](README_PL.md) • [🇬🇧 English](README_EN.md)

**Lekki downloader skryptów Skript bezpośrednio z GitHuba.**

</div>

---

## ✨ Funkcje

- 📥 **GitHub Downloader** — pobieranie plików `.sk` z GitHuba.
- 🔗 **Własne linki** — pobieranie przez bezpośrednie linki GitHub Raw.
- 📂 **Automatyczny zapis** — pliki trafiają do folderu `downloaded`.
- 🔄 **Automatyczne przeładowanie** — przeładowanie pobranego skryptu.
- 🏷️ **Własne nazwy** — możliwość nadania plikowi własnej nazwy.
- 🛡️ **Walidacja URL** — ograniczenie linków do `raw.githubusercontent.com`.
- 🎨 **Kolorowe komunikaty** — czytelne wiadomości w grze i konsoli.

## 📦 Wymagania

| Zależność | Wersja |
|---|---|
| Minecraft | 1.21.5 |
| Java | 21+ |
| Skript | 2.17+ |
| skJson | 5.6.0 |
| skript-reflect | 2.6.2 |

## 📥 Instalacja

1. Pobierz wymagane dodatki.
2. Umieść pliki `.jar` w folderze `plugins`.
3. Pobierz `SkPep.sk`.
4. Umieść go w `plugins/Skript/scripts/`.
5. Wykonaj:

```text
/sk reload SkPep.sk
```

## ⚙️ Konfiguracja

```vb
options:
    prefix: §f[§bSkPep§f]
    repo: https://raw.githubusercontent.com/Pindoza/SkPep/main/scripts/
```

## 💻 Komendy

| Komenda | Opis |
|---|---|
| `/pep <nazwa>` | Pobiera skrypt z repozytorium |
| `/pep <nazwa>.sk` | Pobiera skrypt z rozszerzeniem |
| `/pep link <URL>` | Pobiera z bezpośredniego linku |
| `/pep link <URL> <nazwa>` | Pobiera pod własną nazwą |
| `/pepreload` | Przeładowuje SkPep |

### Przykłady

```text
/pep example
/pep example.sk
/pep link https://raw.githubusercontent.com/Pindoza/SkPep/main/scripts/example.sk
/pep link https://raw.githubusercontent.com/Pindoza/SkPep/main/scripts/example.sk custom
```

## 📁 Struktura repozytorium

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

## 📚 Dostępne skrypty

Wszystkie publiczne skrypty do pobrania znajdują się w folderze:

`/scripts/`

Dodawanie nowych skryptów:

1. Umieść plik `.sk` w folderze `scripts/`.
2. Wypchnij zmiany na GitHub.
3. Pobierz go na serwerze przez `/pep <nazwa>`.

## 📂 Lokalizacja pobranych plików

```text
plugins/Skript/scripts/downloaded/
```

## 🔐 Uprawnienia

| Uprawnienie | Opis |
|---|---|
| `skpep.use` | Dostęp do komend SkPep |

## ⚠️ Bezpieczeństwo

- Pobieraj skrypty wyłącznie z zaufanych źródeł.
- Pliki Skript mogą wykonywać kod na serwerze.
- Sprawdzaj kod przed instalacją.
- Nie instaluj nieznanych skryptów na produkcyjnym serwerze.

---

<div align="center">

**⚡ SkPep — Download. Install. Reload.**

</div>
