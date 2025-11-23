---
title: Incontro 02 - Architetture Cognitive e Custom Agents
description: "Programma dettagliato dell'incontro 02"
tags: [incontro, grafica,]
date: "mar. 09/12/2025"
---

# Incontro 02 - Architetture Cognitive e Custom Agents

- Durata Totale: 4 Ore (pomodoro 50/10/15)
- Focus: Costruire l'infrastruttura digitale del progetto. Creare una base di conoscenza affidabile (NotebookLM) e configurare lo staff virtuale (Gems).

---

### POMODORO 1: Teoria dell'Architettura (50 min)

*Perché l'IA generica non basta e come costruiamo un "Cervello Esterno".*

**1. Il Problema della "Tabula Rasa"**

Quando aprite una chat di Gemini, il modello non sa nulla del vostro progetto, del Liceo Mengaroni o del brief. È un genio senza memoria.
* **Rischio:** Risposte generiche, cliché, allucinazioni sui dati.
* **Soluzione:** Dobbiamo fornire un **Context Window** (Finestra di Contesto) satura di informazioni reali.

**2. La Strategia RAG (Retrieval-Augmented Generation) Semplificata**

Il concetto è semplice:
* Invece di chiedere all'IA di *inventare* una risposta...
* Le chiediamo di *cercare* la risposta nei documenti che le forniamo.
* **Strumento:** Qui entra in gioco **Google NotebookLM**. Non è un generatore, è un analista delle fonti.

**3. Introduzione a GEM e NotebookLM**

- Introduzione alla interfaccia di controllo di Gemini.
- Introduzione alla creazione di GEM.
- Introduzione alla creazione di Notebook LM.


---

☕ **PAUSA BREVE (10 min)**

---

### POMODORO 2: Costruzione della Base di Conoscenza (50 min)

*Hands-on su Google NotebookLM.*

**1. Setup del Notebook (10 min)**
* Accedere a [notebooklm.google.com](https://notebooklm.google.com).
* Creare un nuovo taccuino rinominandolo con il nome del Gruppo/Progetto.

**2. Ingestione dei Dati (In-Feeding) (20 min)**
Ogni gruppo deve caricare le proprie fonti, ad esempio:
* Il PDF del brief di progetto.
* Documenti sulla storia/visione (es. testi su Massimo Dolcini o storia della scuola).
* Reference testuali o appunti di stile.
* *Nota:* NotebookLM "legge" solo il testo, non "guarda" le immagini (per ora).

**3. Interrogare la Fonte (20 min)**
Esercizio pratico: "Intervistare il proprio NotebookLM".
* Usare la chat di NotebookLM per estrarre i vincoli.
* *Prompt di test:* "Estrai una lista puntata di tutti i vincoli tecnici obbligatori presenti nel brief".
* *Prompt di test:* "Quali sono i valori chiave che dovremmo comunicare?".

---

**PAUSA LUNGA (15 min)**

---

### POMODORO 3: Progettare lo Staff (Gems - Parte 1) (50 min)

*Creazione dell'Agente Strategico in Gemini Advanced.*

**1. Introduzione ai Gem**
I Gem sono versioni personalizzate di Gemini. Hanno istruzioni fisse, una personalità definita e un obiettivo unico.
Non dobbiamo ripetere ogni volta "agisci come un esperto di marketing...". Lo settiamo una volta per tutte.

**2. Creazione del Gem "Art Director"**
* **Ruolo:** Visual Lead / Art Director.
* **Obiettivo:** Suggerire concept grafici per tutti i touchpoint (Manifesti, Pieghevoli, Digital).
* **System Instruction (Copia-Incolla da adattare):**
    > "Sei l'Art Director dello Studio [Nome Gruppo]. La tua missione è tradurre concetti astratti in soluzioni visive impattanti.
    > **Le tue Responsabilità:**
    > 1. Proporre stili visivi coerenti (es. Swiss Style, Brutalist, Minimal).
    > 2. Descrivere dettagliatamente layout e composizioni per i vari formati.
    > 3. Definire palette colori (codici HEX se richiesti) e accoppiamenti tipografici.
    > **Vincolo Assoluto:** NON SCRIVERE MAI I TESTI (headline o body copy). Per le parti testuali usa 'Lorem Ipsum' o scrivi '[Qui va la Headline]'. Concentrati solo sull'estetica."

**3. Testing e Tuning (15 min)**
Dialogare con la Gem Art Director.
* Copiare i vincoli tecnici estratti da NotebookLM (Pomodoro 2) e incollarli nella chat.
* Chiedere: "Basandoti su questi vincoli, proponi 3 concept visivi diversi per il manifesto 70x100 dell'Open Day. Descrivi l'immagine principale, la posizione del logo e la scelta tipografica".

**3. Testing e Tuning (15 min)**
Dialogare con la Gem appena creata.
* Copiare i punti chiave estratti da NotebookLM (Pomodoro 2) e incollarli nella chat con la Gem Strategist.
* Chiedere: "Basandoti su questi dati, definisci 3 possibili direzioni strategiche per il progetto".

---

☕ **PAUSA BREVE (10 min)**

---

### POMODORO 4: Espandere il team creativo (50 min)
*Creazione dell'Agente Creativo e simulazione del flusso completo.*

**1. Creazione dell'agente Copywriter**
Creiamo il secondo assistente.
* **Ruolo:** Creative Copywriter.
* **Obiettivo:** Scrivere slogan, headline e testi emotivi.
* **System Instruction (Copia-Incolla da adattare):**
    > "Sei il Lead Copywriter dello Studio [Nome Gruppo]. Il tuo stile è [es. ironico/istituzionale/poetico]. Il tuo compito è trasformare le strategie in parole memorabili. Evita cliché e frasi fatte. Sii audace."

**2. Primo test**
Simuliamo un flusso reale di agenzia:
1.  **NotebookLM:** Fornisce i fatti (Il Brief).
2.  **Gem Strategist:** Elabora la direzione ("Dobbiamo puntare sull'inclusività").
3.  **Gem Copywriter:** Genera l'output (Tutti protagonisti, nessuno escluso").

**3. Debriefing**
Ogni gruppo deve salvare in una cartella Drive un documento contenente:
* Informazioni strategiche ricavate da NotebookLM.
* Informazioni strategiche ricavate dal Gem Strategist.
* Proposte di head ricavate dal Gem Copywriter.

---

*Ultima modifica: dom. 23/11/2025*

