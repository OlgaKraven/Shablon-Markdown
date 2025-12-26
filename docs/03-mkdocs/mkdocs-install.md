# Установка библиотек (MkDocs Material)

## 1. Предварительные требования

Убедитесь, что установлены:
- Python 3.8+
- pip

Проверка:

```bash
python --version
pip --version
```

(на Windows допустимо использовать `py`)

---

## 2. Установка MkDocs Material (рекомендуемый способ)

```bash
pip install mkdocs-material
```

Если используется несколько версий Python:

```bash
python -m pip install mkdocs-material
```

или (Windows):

```bash
py -m pip install mkdocs-material
```

---

## 3. Проверка установки

```bash
mkdocs --version
```

Ожидаемый вывод, например:

`mkdocs, version 1.6.x`

---

## 4. Частые проблемы

### Команда mkdocs не найдена
Причина: путь к `Scripts` (Windows) не в PATH.

Решение:

```bash
python -m mkdocs --version
```

или используйте виртуальное окружение.
