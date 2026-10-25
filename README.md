<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=220&section=header&text=CI%2FCD%20Learning%20Projects&fontSize=44&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=push%20%E2%80%A2%20lint%20%E2%80%A2%20test%20%E2%80%A2%20build%20%E2%80%A2%20deploy&descSize=18&descAlignY=58" width="100%" alt="header"/>

<a href="https://github.com/ChrisRedfield48">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1200&color=00D4FF&center=true&vCenter=true&width=720&height=50&lines=Пять+языков.+Пять+пайплайнов.;Один+принцип:+push+→+lint+→+test+→+build;GitHub+Actions+·+Docker+·+GitHub+Pages;Go+·+Rust+·+PHP+·+C%2B%2B+·+C%23+·+React+·+Fyne" alt="Typing SVG" />
</a>

<br/>

<a href="https://github.com/ChrisRedfield48?tab=repositories"><img alt="Repos" src="https://img.shields.io/badge/репозиториев-20%2B-0A84FF?style=for-the-badge&logo=github&logoColor=white"></a>
<img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white">
<img alt="Docker" src="https://img.shields.io/badge/Docker-контейнеры-2496ED?style=for-the-badge&logo=docker&logoColor=white">
<img alt="Pages" src="https://img.shields.io/badge/GitHub-Pages-222222?style=for-the-badge&logo=githubpages&logoColor=white">

<br/><br/>

<b>
<a href="#deploy">🚀 Deploy</a> &nbsp;•&nbsp;
<a href="#fullstack">🎬 Фуллстек</a> &nbsp;•&nbsp;
<a href="#gui">🆕 GUI</a> &nbsp;•&nbsp;
<a href="#core">📦 Основные</a> &nbsp;•&nbsp;
<a href="#other">🗂️ Остальные</a> &nbsp;•&nbsp;
<a href="#pipelines">⚙️ Пайплайны</a>
</b>

</div>

<br/>

## 📊 В цифрах

<div align="center">

| 🗃️ Репозиториев | 🧬 Языков и стеков | 🖥️ Платформ для бинарников | 🔁 Типов пайплайнов |
|:---:|:---:|:---:|:---:|
| **21** | **10+** | **4** | **3** |
| учебные и боевые | Go · Rust · PHP · C++ · C# · TS · Python · Java · JS | Linux · macOS (Intel + ARM) · Windows | CI · Release · Deploy |

</div>

---

<a id="deploy"></a>

## 🚀 CI/CD (Deploy)

> Полноценный Continuous Deployment: автоматические проверки и публикация на **GitHub Pages**.

<div align="center">

| Проект | Стек | Что делает | Пайплайн | Ссылка |
|:---|:---|:---|:---|:---:|
| ⚡ **cyberpunk-pages** | ![HTML](https://img.shields.io/badge/HTML%20%2F%20CSS%20%2F%20JS-E34F26?style=flat-square&logo=html5&logoColor=white) | Многостраничный фан-сайт Cyberpunk 2077 с глитч-анимациями | `lint` → `deploy to Pages` | [**открыть →**](https://github.com/ChrisRedfield48/cyberpunk-pages) |
| 🚀 **hello-pages** | ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![TS](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white) | SPA-приложение с покрытием тестами | `lint` → `type-check` → `test` → `build` → `deploy` | [**открыть →**](https://github.com/ChrisRedfield48/hello-pages) |

</div>

---

<a id="fullstack"></a>

## 🎬 Фуллстек веб-приложения

> Клиент-серверная архитектура, база данных и контейнеризация.

<div align="center">

| Проект | Стек | Что делает | Пайплайн | Ссылка |
|:---|:---|:---|:---|:---:|
| 🎬 **my-videoeditor** | ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Postgres](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) | Форк AI-видеоредактора **Kimu**, адаптированный для локального запуска: правки под Postgres 18, Nginx и Cloudflare R2 | `format-check` → _build в разработке_ | [**открыть →**](https://github.com/ChrisRedfield48/my-videoeditor) |

</div>

---

<a id="gui"></a>

## 🆕 GUI-проекты · Go + Fyne

> Кроссплатформенные десктопные приложения. Бинарники публикуются в **GitHub Releases** по тегу `v*`.

<div align="center">

| Проект | Стек | Что делает | Пайплайн | Ссылка |
|:---|:---|:---|:---|:---:|
| 🛠 **arduino-manager-gui** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Fyne](https://img.shields.io/badge/Fyne-1A6BAA?style=flat-square) | Менеджер Arduino-библиотек и ядер с поиском по GitHub | `matrix build` → `release` (4 платформы) | [**открыть →**](https://github.com/ChrisRedfield48/arduino-manager-gui) |
| ⚡ **hex-loader** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Fyne](https://img.shields.io/badge/Fyne-1A6BAA?style=flat-square) | Загрузчик HEX-файлов в Arduino через `arduino-cli` | `matrix build` → `release` (4 платформы) | [**открыть →**](https://github.com/ChrisRedfield48/hex-loader) |
| 🎨 **hello-gui** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Fyne](https://img.shields.io/badge/Fyne-1A6BAA?style=flat-square) | Учебное GUI-приложение с автодеплоем бинарников | `matrix build` → `release` | [**открыть →**](https://github.com/ChrisRedfield48/hello-gui) |

<sub>🐧 Linux &nbsp;·&nbsp; 🍎 macOS Intel &nbsp;·&nbsp; 🍏 macOS ARM &nbsp;·&nbsp; 🪟 Windows</sub>

</div>

---

<a id="core"></a>

## 📦 Основные CI/CD-проекты

> Пять репозиториев, пять языков, один и тот же подход: **lint → test → build**.

<div align="center">

| Проект | Язык | Пайплайн | Ссылка |
|:---|:---|:---|:---:|
| 🐹 **my-go-app** | ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) | `vet` → `test` → `docker build` | [**открыть →**](https://github.com/ChrisRedfield48/my-go-app) |
| 🦀 **my-rust-app** | ![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white) | `clippy` → `test` → `docker build` | [**открыть →**](https://github.com/ChrisRedfield48/my-rust-app) |
| 🐘 **my-php-app** | ![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white) | `lint` → `phpunit` → `docker build` | [**открыть →**](https://github.com/ChrisRedfield48/my-php-app) |
| ⚙️ **my-cpp-app** | ![C++](https://img.shields.io/badge/C%2B%2B%20%2F%20CMake-00599C?style=flat-square&logo=cplusplus&logoColor=white) | `clang-format` → `gtest` → `docker build` | [**открыть →**](https://github.com/ChrisRedfield48/my-cpp-app) |
| 🎯 **hello-csharp** | ![.NET](https://img.shields.io/badge/C%23%20%2F%20.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white) | `test` → **release** (matrix-бинарники) | [**открыть →**](https://github.com/ChrisRedfield48/hello-csharp) |

</div>

---

<a id="other"></a>

## 🗂️ Остальные репозитории

> Учебные проекты, где я тренировался в отдельных технологиях. Пайплайны упрощённые или отсутствуют.

<details>
<summary><b>📂 Показать все 10 репозиториев</b></summary>

<br/>

| Проект | Стек | Ссылка |
|:---|:---|:---:|
| 🌌 **hello-static** | HTML + CSS + JS | [открыть →](https://github.com/ChrisRedfield48/hello-static) |
| 🐍 **hello-python** | Python | [открыть →](https://github.com/ChrisRedfield48/hello-python) |
| 🐍 **my-python-app** | Python | [открыть →](https://github.com/ChrisRedfield48/my-python-app) |
| 🐹 **hello-go** | Go | [открыть →](https://github.com/ChrisRedfield48/hello-go) |
| 🐹 **hello-go-releases** | Go | [открыть →](https://github.com/ChrisRedfield48/hello-go-releases) |
| 🦀 **hello-rust** | Rust | [открыть →](https://github.com/ChrisRedfield48/hello-rust) |
| 🦀 **my-rust-app2** | Rust · Dockerfile | [открыть →](https://github.com/ChrisRedfield48/my-rust-app2) |
| ☕ **hello-java** | Java | [открыть →](https://github.com/ChrisRedfield48/hello-java) |
| 🟩 **my-node-app** | JavaScript · Node.js | [открыть →](https://github.com/ChrisRedfield48/my-node-app) |
| 🧪 **my-first-cicd** | первый эксперимент с CI/CD | [открыть →](https://github.com/ChrisRedfield48/my-first-cicd) |

</details>

---

<a id="pipelines"></a>

## ⚙️ Как устроены пайплайны

<table>
<tr>
<td width="33%" valign="top">

### 🔍 CI
**Основные 5 проектов**

- Триггер: `push` и `pull_request`
- Линтинг под свой стек
- Прогон unit-тестов
- Сборка Docker-образа

</td>
<td width="33%" valign="top">

### 📤 Release
**GUI-проекты и `hello-csharp`**

- Триггер: git-тег `v1.0.0`
- Матричная сборка бинарников
- Автопубликация в GitHub Releases

</td>
<td width="33%" valign="top">

### 🌐 Deploy
**Pages-проекты**

- Триггер: `push` в `main`
- Линтинг (и тесты для SPA)
- Публикация статики или `dist/` в GitHub Pages

</td>
</tr>
</table>

### 🧭 Общая схема

```mermaid
flowchart LR
    subgraph CI["🔍 CI"]
        direction LR
        A["push / PR"] --> B["lint"] --> C["test"] --> D["docker build"]
    end

    subgraph REL["📤 Release"]
        direction LR
        E["git tag v*"] --> F["build matrix"]
        F --> G["linux-amd64"]
        F --> H["darwin-amd64"]
        F --> I["darwin-arm64"]
        F --> J["windows-amd64"]
        G --> K["GitHub Release"]
        H --> K
        I --> K
        J --> K
    end

    subgraph DEP["🌐 Deploy"]
        direction LR
        L["push to main"] --> M["CI: lint & test"]
        M -->|success| N["GitHub Pages"]
    end

    classDef start fill:#2088FF,stroke:#1a6fd6,color:#fff;
    classDef done fill:#00d4ff,stroke:#00a8cc,color:#000;
    class A,E,L start;
    class D,K,N done;
```

---

<div align="center">

### 👤 [ChrisRedfield48](https://github.com/ChrisRedfield48)

<sub>Кликни по названию проекта в любой таблице — попадёшь в репозиторий с кодом, README и историей запусков workflow.</sub>

<br/><br/>

<a href="https://github.com/ChrisRedfield48?tab=repositories"><img src="https://img.shields.io/badge/📂-Все%20репозитории-0A84FF?style=for-the-badge" alt="repos"></a>
<a href="https://github.com/ChrisRedfield48?tab=repositories&type=source"><img src="https://img.shields.io/badge/🛠-Проекты-2088FF?style=for-the-badge" alt="projects"></a>
<a href="https://github.com/ChrisRedfield48?tab=stars"><img src="https://img.shields.io/badge/⭐-Избранное-F5B301?style=for-the-badge" alt="stars"></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=110&section=footer" width="100%" alt="footer"/>

</div>