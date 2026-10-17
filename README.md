# 🚀 CI/CD Learning Projects

<p align="center">
  <b>Пять языков. Пять пайплайнов. Один принцип: push → lint → test → build.</b>
</p>

<p align="center">
  <a href="https://github.com/ChrisRedfield48?tab=repositories">
    <img alt="Repos" src="https://img.shields.io/badge/repos-20%2B-blue?style=for-the-badge">
  </a>
  <img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white">
</p>

---

## 🌐 Статические сайты и SPA (GitHub Pages)

> Проекты с автоматическим деплоем на GitHub Pages (Environments + Deployments). Без сборки или со сборкой, но всегда с гейтингом `needs: ci`.

| Проект | Стек | Что делает | CI/CD | Репозиторий |
|---|---|---|---|---|
| ⚡ **cyberpunk-pages** | HTML + CSS + JS | Многостраничный фан-сайт Cyberpunk 2077 с глитч-анимациями | lint → deploy to Pages | [открыть →](https://github.com/ChrisRedfield48/cyberpunk-pages) |
| 🚀 **hello-pages** | React + TS + Vite | SPA-приложение с покрытием тестами | lint → type-check → test → build → deploy | [открыть →](https://github.com/ChrisRedfield48/hello-pages) |
| 🌌 **hello-static** | HTML + CSS + JS | Многостраничный сайт с интерактивным 3D-фоном | lint → deploy to Pages | [открыть →](https://github.com/ChrisRedfield48/hello-static) |

---

## 🆕 Новые GUI-проекты (Go + Fyne)

> Кроссплатформенные десктопные приложения с публикацией бинарников в GitHub Releases.

| Проект | Стек | Что делает | CI/CD | Репозиторий |
|---|---|---|---|---|
| 🛠 **arduino-manager-gui** | Go + Fyne | Менеджер Arduino-библиотек и ядер с поиском по GitHub | matrix build → release (4 платформы) | [открыть →](https://github.com/ChrisRedfield48/arduino-manager-gui) |
| ⚡ **hex-loader** | Go + Fyne | Загрузчик HEX-файлов в Arduino через arduino-cli | matrix build → release (4 платформы) | [открыть →](https://github.com/ChrisRedfield48/hex-loader) |
| 🎨 **hello-gui** | Go + Fyne | Учебное GUI-приложение с автодеплоем бинарников | matrix build → release | [открыть →](https://github.com/ChrisRedfield48/hello-gui) |

> Все три проекта собираются под **Linux / macOS (Intel + ARM) / Windows** и публикуются в **GitHub Releases** по тегу `v*`.

---

## 📦 Основные CI/CD-проекты

> Пять репозиториев с полноценным пайплайном **lint → test → build**. Каждый — на своём языке.

| Проект | Стек | Пайплайн | Репозиторий |
|---|---|---|---|
| 🐹 **my-go-app** | Go | vet → test → docker build | [открыть →](https://github.com/ChrisRedfield48/my-go-app) |
| 🦀 **my-rust-app** | Rust | clippy → test → docker build | [открыть →](https://github.com/ChrisRedfield48/my-rust-app) |
| 🐘 **my-php-app** | PHP | lint → phpunit → docker build | [открыть →](https://github.com/ChrisRedfield48/my-php-app) |
| ⚙️ **my-cpp-app** | C++ / CMake | clang-format → gtest → docker build | [открыть →](https://github.com/ChrisRedfield48/my-cpp-app) |
| 🎯 **hello-csharp** | C# / .NET | test → **release** (matrix binaries) | [открыть →](https://github.com/ChrisRedfield48/hello-csharp) |

---

## 🗂️ Остальные репозитории

> Учебные проекты, где я тренировался в отдельных технологиях. Пайплайны упрощённые или отсутствуют.

| Проект | Стек | Репозиторий |
|---|---|---|
| 🐍 **hello-python** | Python | [открыть →](https://github.com/ChrisRedfield48/hello-python) |
| 🐍 **my-python-app** | Python | [открыть →](https://github.com/ChrisRedfield48/my-python-app) |
| 🐹 **hello-go** | Go | [открыть →](https://github.com/ChrisRedfield48/hello-go) |
| 🐹 **hello-go-releases** | Go | [открыть →](https://github.com/ChrisRedfield48/hello-go-releases) |
| 🦀 **hello-rust** | Rust | [открыть →](https://github.com/ChrisRedfield48/hello-rust) |
| 🦀 **my-rust-app2** | Rust / Dockerfile | [открыть →](https://github.com/ChrisRedfield48/my-rust-app2) |
| ☕ **hello-java** | Java | [открыть →](https://github.com/ChrisRedfield48/hello-java) |
| 🟩 **my-node-app** | JavaScript / Node.js | [открыть →](https://github.com/ChrisRedfield48/my-node-app) |
| 🧪 **my-first-cicd** | — | [открыть →](https://github.com/ChrisRedfield48/my-first-cicd) |

---

## ⚙️ Как устроены пайплайны

### 🔍 CI — в основных пяти проектах

- Триггер: `push` и `pull_request`
- Статический анализ / линтинг под свой стек
- Прогон unit-тестов
- Сборка Docker-образа приложения

### 📤 Release — в GUI-проектах и `hello-csharp`

- Триггер: push git-тега (`v1.0.0` и т.п.)
- Матричная сборка self-contained бинарников
- Автопубликация в GitHub Releases

### 🌐 Deploy to Pages — в статических сайтах и SPA

- Триггер: `push` в ветку `main`
- Линтинг (и тесты для SPA)
- Прямая публикация статики (или папки `dist/`) в GitHub Pages

### Диаграмма пайплайнов

```mermaid
flowchart LR
    A[push / PR] --> B[lint]
    B --> C[test]
    C --> D[docker build]

    E[git tag v*] --> F[build matrix]
    F --> G[linux-amd64]
    F --> H[darwin-amd64]
    F --> I[darwin-arm64]
    F --> J[windows-amd64]
    G --> K[GitHub Release]
    H --> K
    I --> K
    J --> K

    L[push to main] --> M[CI: lint & test]
    M -->|success| N[deploy to GitHub Pages]

    style A fill:#2088FF,color:#fff
    style E fill:#ff2e88,color:#fff
    style L fill:#2088FF,color:#fff
    style K fill:#00d4ff,color:#000
    style N fill:#00d4ff,color:#000
```

---

## 🧭 Навигация

> Кликни по названию проекта в любой таблице — попадёшь прямо в репозиторий с полным README, кодом и историей запусков workflow.

### 👤 [ChrisRedfield48](https://github.com/ChrisRedfield48)

---

<p align="center">
  <a href="https://github.com/ChrisRedfield48?tab=repositories">📂 Все репозитории</a> ·
  <a href="https://github.com/ChrisRedfield48?tab=repositories&type=source">🛠 Проекты</a> ·
  <a href="https://github.com/ChrisRedfield48?tab=stars">⭐ Избранное</a>
</p>