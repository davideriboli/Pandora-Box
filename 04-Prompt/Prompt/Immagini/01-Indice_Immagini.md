---
title: Indice Prompt
description: "Indice di sezione"
tags: [prompt, indici]
date: "2025-05-11"
---

# Prompt per Creazione Immagini

```dataview
TABLE WITHOUT ID
    file.link AS "Titolo File",
    description AS "Descrizione"
FROM "04-Prompt/Prompt/Immagini/Varia"
WHERE file.name != this.file.name AND file.ext = "md"
SORT file.name ASC
```

---