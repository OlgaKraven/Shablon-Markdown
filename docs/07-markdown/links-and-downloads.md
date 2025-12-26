# Гиперссылки и скачивание файлов в Markdown

Ниже приведены корректные примеры кода для создания гиперссылок в Markdown (.md), включая базовые и расширенные варианты, используемые в учебной и проектной документации.

---

## 1. Базовая гиперссылка
```markdown
[Официальный сайт Python](https://www.python.org)
```

---

## 2. Гиперссылка с поясняющим текстом
```markdown
Перейдите на [официальную документацию MkDocs](https://www.mkdocs.org) для изучения возможностей системы.
```

---

## 3. Открытие в новой вкладке (MkDocs Material)
```markdown
[Открыть документацию Python](https://www.python.org){: target="_blank" rel="noopener" }
```

---

## 4. Ссылка на страницу внутри проекта MkDocs
```markdown
[Введение](theory/introduction.md)
```

---

## 5. Ссылка на раздел страницы (якорь)
```markdown
[Перейти к разделу "Практика"](#практика)
```

---

## 6. Клик по изображению (ссылка-картинка)
```markdown
[![ER-диаграмма](img/er.png)](img/er.png)
```

---

## 7. Ссылка в виде кнопки (Material)
```markdown
[Скачать шаблон отчёта](files/report-template.docx){: .md-button .md-button--primary }
```

---

## 8. Скачивание файлов (download)

### 8.1 Простая ссылка на скачивание
```markdown
[Скачать шаблон отчёта](files/report-template.docx)
```

### 8.2 Принудительное скачивание
```markdown
[Скачать шаблон отчёта](files/report-template.docx){: download }
```

### 8.3 Кнопка «Скачать» (рекомендуется)
```markdown
[Скачать шаблон отчёта](files/report-template.docx){: .md-button .md-button--primary download }
```

### 8.4 Скачивание PDF
```markdown
[Скачать методические указания (PDF)](files/methodical-guidelines.pdf){: download }
```

### 8.5 Скачивание ZIP
```markdown
[Скачать архив проекта](files/project-source.zip){: download }
```

---

## 9. Рекомендации по структуре файлов

Рекомендуемая структура:

```text
docs/
└─ files/
   ├─ report-template.docx
   ├─ project-source.zip
   └─ guidelines.pdf
```
