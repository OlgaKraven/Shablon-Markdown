# Проверка установленного Python

## 1. Универсальный способ (Windows, macOS, Linux)

Откройте терминал:

- **Windows:** Win + R → `cmd` или PowerShell  
- **macOS:** Terminal  
- **Linux:** любой терминал  

Выполните команду:

```bash
python --version
```

или:

```bash
python3 --version
```

## Возможные результаты

- `Python 3.x.x` — Python установлен
- `command not found` / «не является внутренней или внешней командой» — Python не установлен или не добавлен в PATH

---

## 2. Проверка на Windows (рекомендуется)

### 2.1 Через Python Launcher

```bash
py --version
```

Если Python установлен корректно, вы увидите, например:

`Python 3.12.1`

> `py` — стандартный способ работы с Python на Windows.

### 2.2 Проверка всех установленных версий

```bash
py -0
```

Пример:

```text
Installed Pythons found by py Launcher:
 -3.12-64
 -3.11-64
```

---

## 3. Проверка на macOS и Linux

### 3.1 Проверка Python 3 (основной вариант)

```bash
python3 --version
```

### 3.2 Проверка пути установки

```bash
which python3
```

Пример:

`/usr/bin/python3`

---

## 4. Проверка через интерактивный режим

Запустите интерпретатор:

```bash
python
```

или

```bash
python3
```

Если Python установлен, вы увидите приглашение вида:

```text
Python 3.12.1 (main, ...)
>>>
```

Выход из режима:

```python
exit()
```

---

## 5. Частые проблемы и решение

### Python установлен, но команда не работает

**Причина:** Python не добавлен в PATH.

Проверка пути (Windows):

```bash
where python
```

**Решение:**
- переустановить Python с галочкой **Add Python to PATH**
- либо добавить путь вручную в переменные среды
