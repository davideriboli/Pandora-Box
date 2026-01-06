---
title: Installare ComfyUI su Arch e derivate
description: Istruzioni dettagliate per l'installazione corretta di ComfyUI su sistemi Arch Linux.
tags:
  - comfy
  - linux
date: "dom. 04/01/2026"
---

## Installare ComfyUI su Arch e derivate

> [!NOTA BENE]
> La data di *ultima modifica* in fondo all’articolo indica l’ultima volta che ho eseguito con successo le istruzioni che seguono. Controllate in anticipo la documentazione ufficiale se volete provarci anche voi, specie se sono passati diversi giorni dalla data indicata.
> Non iniziate neppure, se non conoscete - almeno a grandi linee - il senso dei comandi indicati.

---

1. Cloniamo lo script (vedete voi dove preferite farlo) e spostiamoci lì dentro.

```bash
git clone https://github.com/comfyanonymous/ComfyUI && cd ComfyUI
```

2. Controlliamo di avere pip installato e aggiornato.

```bash
sudo pacman -S python-pip
```

3. Creazione del venv.

```python
python -m venv venv
```

4. Attivazione del venv.

```python
source venv/bin/activate
```

5. **ATTENZIONE!** Questo vale per la mia macchina con nVidia GeForce RTX 4090 e, in generale per tutte le nVidia. Se avete GPU AMD o altro, dovete trovare il vostro elenco di librerie e script.

```python
pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu124
```

6. Ora installiamo la roba che serve a ComfyUI.

```python
pip install -r requirements.txt
```

7. Finito. Lo script si lancia con:

```python
python main.py
```

8. E si ferma con `CTRL+C` in terminale e poi:

```python
deactivate
```

9. Per tenere aggiornato lo script è sufficiente fare un `git pull` dal *repository* ufficiale.

---

*Ultima modifica: dom. 04/01/2026*

