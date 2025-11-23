# Dispensa & Programma: Incontro 02
## Architetture Cognitive e Custom Agents
**Liceo Artistico "Ferruccio Mengaroni" - Didattica del Progetto Grafico & IA**

**Obiettivo:** Costruire l'infrastruttura digitale del progetto. Creare una base di conoscenza affidabile (NotebookLM) e configurare lo staff virtuale (Gems) con focus sulla Direzione Artistica e il Copywriting.

---

### 🍅 POMODORO 1: Teoria dell'Architettura (50 min)
*Perché l'IA generica non basta e come costruiamo un "Cervello Esterno".*

**1. Il Problema della "Tabula Rasa" (15 min)**
Quando aprite una chat di Gemini, il modello non sa nulla del vostro progetto, del Liceo Mengaroni o del brief. È un genio creativo, ma senza memoria.
* **Rischio:** Risposte generiche, cliché visivi, allucinazioni sui dati.
* **Soluzione:** Fornire un **Context Window** satura di informazioni reali tramite NotebookLM.

**2. La Strategia RAG (Retrieval-Augmented Generation) Semplificata (20 min)**
Il concetto chiave per i designer:
* Invece di chiedere all'IA di *inventare* dal nulla...
* Le chiediamo di *elaborare* i documenti che le forniamo.
* **NotebookLM** diventa il nostro "Account Manager": conosce a memoria il brief, i vincoli tecnici e i desideri del cliente.

**3. Visualizzazione del Flusso (15 min)**
Immaginate il flusso di lavoro come uno studio grafico strutturato:
* **L'Archivio (NotebookLM):** Dove risiedono i vincoli (Formati, Budget, Scadenze, Storia).
* **I Creativi (Gems):** Gli agenti (Art Director e Copywriter) che usano quei vincoli per creare.

> **🖼️ Prompt Visual 01 (L'Architetto):**
> `Minimalist 3D isometric diagram. Left side: A stack of paper documents and PDF icons entering a glowing funnel. Center: A clean, white digital brain structure (representing NotebookLM). Right side: Multiple colored beams of light exiting the brain and connecting to different robot avatars (representing Agents). White background, clean tech aesthetic, soft blue and orange lighting. --ar 16:9`

---

☕ **PAUSA BREVE (10 min)**

---

### 🍅 POMODORO 2: Costruzione della Base di Conoscenza (50 min)
*Hands-on su Google NotebookLM.*

**1. Setup del Notebook (10 min)**
* Accedere a [notebooklm.google.com](https://notebooklm.google.com).
* Creare un nuovo taccuino rinominandolo con il nome del Gruppo (es. *"Studio Alpha - Brief Mengaroni"*).

**2. Ingestione dei Dati (In-Feeding) (20 min)**
Ogni gruppo carica le fonti raccolte nel Modulo 1:
* PDF del Brief.
* Documenti storici (es. Dolcini/Pesaro).
* Reference di brand (Brand manual esistenti se presenti).

**3. Interrogare la Fonte (20 min)**
Esercizio "Intervista il Brief":
* Usare la chat di NotebookLM per estrarre i vincoli *non negoziabili*.
* *Prompt di test:* "Estrai una lista dei formati richiesti (es. manifesto 70x100, post Instagram) e dei loghi obbligatori."
* *Prompt di test:* "Qual è il tono di voce richiesto dal cliente? Formale, giovanile, istituzionale?"

> **🖼️ Prompt Visual 02 (L'Analista):**
> `Close-up of a futuristic digital interface on a glass tablet. The screen shows a document being scanned by a beam of light, extracting key sentences which are floating up and organizing themselves into a neat list. Data visualization, holographic effect, dark mode UI, cyan neon accents. --ar 16:9`

---

🥪 **PAUSA LUNGA (15 min)**

---

### 🍅 POMODORO 3: Progettare lo Staff (Gems - Parte 1) (50 min)
*Creazione dell'Agente "ART DIRECTOR" in Gemini Advanced.*

**1. Il Ruolo dell'Art Director Virtuale (10 min)**
Non stiamo creando un generatore di immagini (quello verrà dopo), ma un **Generatore di Idee Visive**.
Questa Gem deve ragionare come un Senior Designer: pensare al layout, alla gerarchia, ai colori e alla tipografia.

**2. Creazione della Gem "ART DIRECTOR" (25 min)**
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

> **🖼️ Prompt Visual 03 (L'Art Director):**
> `Portrait of a creative AI avatar representing an 'Art Director'. The figure is surrounded by floating color palettes, typography samples, and grid systems. The avatar holds a digital stylus. Expressive, colorful, artistic atmosphere but professional. Background is a blurred design studio. --ar 16:9`

---

☕ **PAUSA BREVE (10 min)**

---

### 🍅 POMODORO 4: Espandere il Team e Workflow (50 min)
*Creazione dell'Agente Copywriter e simulazione del flusso completo.*

**1. Creazione dell'Agente "COPYWRITER" (20 min)**
Creiamo il partner dell'Art Director.
* **Ruolo:** Creative Copywriter.
* **Obiettivo:** Riempire i layout dell'Art Director con parole memorabili.
* **System Instruction:**
    > "Sei il Lead Copywriter. Il tuo compito è scrivere headline, slogan e body copy. Il tuo tono deve adattarsi allo stile visivo proposto dall'Art Director. Sii sintetico e persuasivo. Non descrivere immagini, scrivi solo il testo."

**2. Il Grande Test: La Staffetta Creativa (20 min)**
Simuliamo il flusso di agenzia:
1.  **NotebookLM:** Estrae il tema ("L'Open Day deve comunicare innovazione").
2.  **Gem Art Director:** Propone il visual ("Un'immagine isometrica della scuola che esplode in pixel colorati. Fondo blu notte. Titolo grande in alto a sinistra in font sans-serif bold").
3.  **Gem Copywriter:** Scrive il testo per *quel* layout ("Headline: Il tuo futuro, pixel dopo pixel. Body: Vieni a progettare il domani al Mengaroni.").
*Gli studenti eseguono questo passaggio copiando l'output di un agente nell'altro.*

**3. Debriefing e Output Finale (10 min)**
Ogni gruppo salva un documento "01_Concept_Board" contenente:
* 3 Proposte di Direzione Artistica (Descrizione visuale).
* 3 Proposte di Headline abbinate.
* Questo materiale sarà la base per la generazione immagini dell'Incontro 3.

> **🖼️ Prompt Visual 04 (Il Team al Lavoro):**
> `A collaborative workspace scene. Three distinct AI avatars sitting around a holographic table working together. One is analyzing data (blue), one is sketching layouts in the air (magenta - Art Director), one is typing text (orange - Copywriter). Synergy, collaboration, creative flow. 8k, highly detailed. --ar 16:9`

---