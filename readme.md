# create-repo

> 🧰 Bash CLI-утилита для быстрого создания GitHub-репозиториев из любой папки

`create-repo` — это простой, но мощный скрипт, который:

- 🔧 Инициализирует git в текущей папке (если ещё не инициализирован)
- 🌱 Создаёт ветку `main`
- 📄 Автоматически генерирует `README.md`, если его нет
- 🧠 Определяет тип проекта и создаёт подходящий `.gitignore` (Node.js, Python, Terraform и др.)
- ☁️ Создаёт репозиторий на GitHub через GitHub CLI (`gh`)
- 🚀 Делает первый коммит и пуш

---

## ⚙️ Требования

- `git`
- `gh` — GitHub CLI (установится автоматически при запуске, если есть `sudo` и интернет)

---

## 🚀 Установка (способ 1 — вручную)

```bash
# 1. Скопируйте файл create-repo на нужную машину
scp create-repo user@remote:/tmp/

# 2. Установите в систему
sudo mv /tmp/create-repo /usr/local/bin/create-repo
sudo chmod +x /usr/local/bin/create-repo
