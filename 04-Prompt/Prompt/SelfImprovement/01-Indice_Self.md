---
title: Indice Prompt
description: "Indice di sezione"
tags: [prompt, indici]
date: "2025-05-11"
---

# Indice Prompt Self

```dataview
TABLE WITHOUT ID
    file.link AS "Titolo File",
    description AS "Descrizione"
FROM "04-Prompt/Prompt/SelfImprovement/Prompt"
WHERE file.name != this.file.name AND file.ext = "md"
SORT file.name ASC
```

---

> [!ATTENZIONE]
> I prompt di *self improvement* vanno sempre usati con estrema cautela e solo dopo averli attentamente e ripetutamente raffinati con l’ultima versione disponibile dell’IA che si intente usare.