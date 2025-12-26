# Установка Python

## Официальный способ (рекомендуется)

1. Перейдите на официальный сайт: https://www.python.org/downloads/  
2. Используйте только официальный сайт во избежание проблем с безопасностью и версиями.

---

## Установка на Windows (рекомендуется для учебных и проектных работ)

### Шаг 1. Скачивание
- Нажмите **Download Python 3.x.x**
- Скачайте установщик `.exe`

### Шаг 2. Запуск установщика
Обязательно:
- ✅ поставьте галочку **Add Python to PATH**
- нажмите **Install Now**

### Шаг 3. Проверка установки
Откройте cmd или PowerShell и выполните:

```bash
py --version
```

или

```bash
python --version
```

Ожидаемый результат:

`Python 3.x.x`

---

## Установка на macOS

### Вариант 1. Через официальный установщик (рекомендуется)
1. Скачайте `.pkg` файл с сайта python.org  
2. Установите Python стандартным способом  
3. Проверьте:

```bash
python3 --version
```

### Вариант 2. Через Homebrew (для продвинутых пользователей)

```bash
brew install python
```

Проверка:

```bash
python3 --version
```

---

## Установка на Linux

### Ubuntu / Debian

```bash
sudo apt update
sudo apt install python3 python3-pip -y
```

### Fedora

```bash
sudo dnf install python3 python3-pip -y
```

### Arch

```bash
sudo pacman -S python python-pip
```

Проверка:

```bash
python3 --version
```

---

## Что устанавливается вместе с Python

- интерпретатор Python  
- `pip` — менеджер пакетов  
- стандартная библиотека  
- (Windows) Python Launcher `py`

---

## После установки рекомендуется

```bash
python -m pip install --upgrade pip
```
