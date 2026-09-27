<div align="center">

# 🚀 CI/CD Learning Projects

**Пять языков. Пять пайплайнов. Один принцип: push → lint → test → build.**

![Go](https://img.shields.io/badge/-Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Rust](https://img.shields.io/badge/-Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![PHP](https://img.shields.io/badge/-PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![C++](https://img.shields.io/badge/-C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![C#](https://img.shields.io/badge/-C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)

</div>

---

## 📦 Проекты

<table>
<tr><th>Проект</th><th>Стек</th><th>Пайплайн</th><th>Репозиторий</th></tr>

<tr>
<td>🐹 <b>my-go-app</b></td>
<td>Go</td>
<td>vet → test → docker build</td>
<td><a href="https://github.com/ChrisRedfield48/my-go-app">открыть →</a></td>
</tr>

<tr>
<td>🦀 <b>my-rust-app</b></td>
<td>Rust</td>
<td>clippy → test → docker build</td>
<td><a href="https://github.com/ChrisRedfield48/my-rust-app">открыть →</a></td>
</tr>

<tr>
<td>🐘 <b>my-php-app</b></td>
<td>PHP</td>
<td>lint → phpunit → docker build</td>
<td><a href="https://github.com/ChrisRedfield48/my-php-app">открыть →</a></td>
</tr>

<tr>
<td>⚙️ <b>my-cpp-app</b></td>
<td>C++ / CMake</td>
<td>clang-format → gtest → docker build</td>
<td><a href="https://github.com/ChrisRedfield48/my-cpp-app">открыть →</a></td>
</tr>

<tr>
<td>🎯 <b>hello-csharp</b></td>
<td>C# / .NET</td>
<td>test → <b>release</b> (matrix binaries)</td>
<td><a href="https://github.com/ChrisRedfield48/hello-csharp">открыть →</a></td>
</tr>

</table>

---

## ⚙️ Как устроены пайплайны

```
push / PR ──▶ lint ──▶ test ──▶ docker build
                                     │
                          (только hello-csharp)
                                     ▼
                        git tag v* ──▶ release
                     matrix: linux-x64 · osx-arm64 · win-x64
```

<details>
<summary><b>🔍 CI — во всех пяти проектах</b></summary>
<br>

- Триггер: push и pull request
- Статический анализ / линтинг под свой стек
- Прогон unit-тестов
- Сборка Docker-образа приложения

</details>

<details>
<summary><b>📤 Release — только hello-csharp</b></summary>
<br>

- Триггер: push git-тега (`v1.0.0` и т.п.)
- Матричная сборка self-contained бинарников: `linux-x64`, `osx-arm64`, `win-x64`
- Автопубликация в GitHub Releases

</details>

---

## 🧭 Навигация

> Кликни по названию проекта в таблице — попадёшь прямо в репозиторий с полным README, кодом и историей запусков workflow.

<div align="center">

### 👤 [ChrisRedfield48](https://github.com/ChrisRedfield48)

</div>