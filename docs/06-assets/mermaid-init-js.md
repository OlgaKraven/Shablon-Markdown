# Создание JavaScript-файла инициализации Mermaid

Для корректного отображения диаграмм Mermaid в документации MkDocs Material используется отдельный JavaScript-файл, который выполняет инициализацию библиотеки после полной загрузки HTML-страницы.

---

## 1. Назначение файла

JavaScript-файл предназначен для:
- безопасной инициализации Mermaid;
- предотвращения ошибок, если библиотека ещё не подключена;
- централизованной настройки параметров визуализации диаграмм.

Файл подключается через параметр `extra_javascript` в `mkdocs.yml`.

---

## 2. Создание файла

В структуре проекта MkDocs создаётся файл:

```text
docs/
└─ js/
   └─ mermaid-init.js
```

---

## 3. Содержимое файла `mermaid-init.js`

```javascript
document.addEventListener("DOMContentLoaded", () => {
  if (window.mermaid) {
    mermaid.initialize({
      startOnLoad: true,
      theme: "default"
    });
  }
});
```

---

## 4. Подключение файла в mkdocs.yml

```yaml
extra_javascript:
  - https://unpkg.com/mermaid@10/dist/mermaid.min.js
  - js/mermaid-init.js
```

Важно:
- сначала подключается библиотека Mermaid;
- затем файл инициализации.
