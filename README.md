# 📒 Go Phonebook

![Go](https://img.shields.io/badge/Go-1.25-00ADD8?style=flat&logo=go&logoColor=white)
![Platform](https://img.shields.io/badge/platform-Linux%20%7C%20macOS%20%7C%20Windows-lightgrey?style=flat)
![Status](https://img.shields.io/badge/status-early%20stage-orange?style=flat)
![License](https://img.shields.io/badge/license-MIT-green?style=flat)


> Учебное приложение для работы с телефонной книгой, написанное на Go.  
> Проект находится на самой ранней стадии разработки 🚀

---

## 📋 О проекте

**Go Phonebook** — простая консольная утилита для хранения и поиска контактов.  
Создана в учебных целях для освоения основ языка Go: структуры данных, аргументы командной строки, срезы и функции.

На данный момент контакты хранятся прямо в коде

---

## 🗂️ Структура контакта

Каждая запись в телефонной книге содержит три поля:

| Поле      | Описание       |
|-----------|----------------|
| `Name`    | Имя контакта   |
| `Surname` | Фамилия        |
| `Tel`     | Номер телефона |

---

## ⚡ Возможности

- 🔍 **Поиск** контакта по фамилии
- 📃 **Список** всех контактов в книге

---

## 🛠️ Как запустить

### 1. Клонируй репозиторий

```bash
git clone https://github.com/skypixie/go-phonebook.git
cd go-phonebook
```

### 2. Собери проект

```bash
go build -o phonebook
```

### 3. Запусти!

```bash
./phonebook
```

Без аргументов программа покажет подсказку:

```
Usage: phonebook search|list <arguments>
```

---

## 📖 Использование

### 📃 Показать все контакты

```bash
./phonebook list
```

**Вывод:**
```
{Mihalis Tsoukalos 2109416471}
{Mary Doe 2109416871}
{John Black 2109416123}
```

### 🔍 Найти контакт по фамилии

```bash
./phonebook search Doe
```

**Вывод:**
```
{Mary Doe 2109416871}
```

### ❌ Контакт не найден

```bash
./phonebook search Smith
```

**Вывод:**
```
Entry not found: Smith
```

---

## 📁 Структура файлов

```
go-phonebook/
└── main.go   # Весь код приложения
```
---