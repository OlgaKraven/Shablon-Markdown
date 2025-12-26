# Плагин material-glightbox (увеличение изображений)

Команда:

```bash
pip install material-glightbox
```

используется для установки плагина **glightbox** для темы MkDocs Material, который добавляет увеличение изображений (lightbox) при клике.

---

## 1. Установка плагина

Рекомендуемый способ (универсально):

```bash
python -m pip install material-glightbox
```

или на Windows:

```bash
py -m pip install material-glightbox
```

Если используете виртуальное окружение — команда выполняется после его активации.

---

## 2. Проверка установки

```bash
pip show material-glightbox
```

---

## 3. Подключение в mkdocs.yml (ОБЯЗАТЕЛЬНО)

```yaml
plugins:
  - search
  - glightbox
```

> Название плагина — `glightbox`, а не `material-glightbox`.

---

## 4. Использование в Markdown

Обычное изображение (будет увеличиваться автоматически):

```markdown
![ER-диаграмма](img/er-diagram.png)
```

Группа изображений (галерея):

```markdown
![Screen 1](img/s1.png)
![Screen 2](img/s2.png)
![Screen 3](img/s3.png)
```
