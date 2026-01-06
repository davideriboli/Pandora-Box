---
title: On Our Own
description: Avvio all'uso dell'IA indipendente e libera
tags:
  - prompt
  - opensource
  - ia
date: "dom. 04/01/2026"
---

## On our own

Non è impossibile, ma è spesso necessario usare sistemi di Intelligenza Artificiale che possano garantire una assoluta riservatezza e siano in grado di produrre artefatti non soggetti a meccanismi censori non controllabili dall’utente.

In questa sezione, sono raccolte le informazioni minime per “provare a far da soli”. Ricordate però che, in questo caso, avrete bisogno di computer piuttosto potenti. Il mio consiglio è:

1. una macchina (non importa se desktop o laptop) a base Windows
2. una scheda grafica nVidia RTX 4090 (minimo)
3. sistema operativo Linux (Arch Linux o EndeavourOS altamente consigliati)

Certo è possibile ottenere risultati anche su macchine meno potenti, magari Macintosh o Windows, ma quasi certamente dovrete fare i conti con problemi vari, malfunzionamenti, lunghe attese e risultati deludenti.

### Principali sistemi chat

1. [LM-Studio](https://lmstudio.ai/) | La base per tutti, lavora con API e modelli Huggingface.
2. [AnythingLLM](https://anythingllm.com/) | Potente sistema RAG che può funzionare anche come chatbot indipendente ed è altamente compatibile con LM-Studio. Anche questo lavora con API e modelli Huggingface. Ne esiste una versione per cellulare che funziona piuttosto bene.
3. [GPT4All](https://www.nomic.ai/gpt4all) | La scelta più facile, ma anche la meno efficace. Lavora essenzialmente con LLM propri e alcuni Huggingface. Buona la capacità RAG, ma neppure paragonabile a quella di AnythingLLM. In compenso, può funzionare (male e molto lentamente, anche su macchine prive di GPU).

### Principali sistemi per immagini e video

1. [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | Probabilmente, l’unica soluzione che al momento meriti di essere citata. Può generare immagini, video, eseguire upscaling e persino creare musica (bruttina). Lavora con ogni genere di LLM dedicato alla creazione multimediale (tipo Stable Diffusion o Flux) ed è disponibile per qualsiasi sistema operativo.
2. [SwarmUI](https://swarmui.net/) | Si basa sempre su Comfy, che ne costituisce il *backend*, ma offre una GUI più semplice per chi non se la cava coi sistemi a nodi.

---

