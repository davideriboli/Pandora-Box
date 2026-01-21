---
title: Claude Prompt Base Test
description: Struttura base dei prompt per Claude in testo corrente.
tags:
  - prompt
  - claude
date: mer. 21/01/2026
---

## Claude Prompt Base in testo corrente

# Prompt Testuali Senza XML: Best Practices

## Principi Fondamentali

### 1. **Usa separatori visivi chiari**

```
===================
SEZIONE PRINCIPALE
===================

-------------------
Sottosezione
-------------------

• Punto importante
• Altro punto
```

### 2. **Sfrutta intestazioni gerarchiche**

```
# LIVELLO 1 - Massima importanza
## Livello 2 - Sezione
### Livello 3 - Dettaglio
```

### 3. **Applica formattazione enfatica**

```
**IMPORTANTE**: istruzioni critiche
*Nota*: informazioni secondarie
TUTTO MAIUSCOLO: elementi chiave da non perdere
```

---

## Struttura Ottimale (Senza XML)

### Template Base:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
CONTESTO E RUOLO
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[Descrizione chiara di chi sei e cosa devi fare]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
DOCUMENTI / DATI DI INPUT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[Il contenuto da analizzare va qui]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
ISTRUZIONI
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Devi seguire queste regole:

1. [Prima regola]
2. [Seconda regola]
3. [Terza regola]

**IMPORTANTE**: [vincoli critici]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
ESEMPI
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Esempio 1:
Input: [esempio input]
Output atteso: [esempio output]

Esempio 2:
Input: [esempio input]
Output atteso: [esempio output]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
LA TUA RICHIESTA SPECIFICA
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[La domanda o il task vero e proprio]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
FORMATO OUTPUT RICHIESTO
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[Specifica come vuoi la risposta]
```

---

## Esempi Pratici

### 1. ANALISI DOCUMENTI

```
═══════════════════════════════════════════════════════════
RUOLO
═══════════════════════════════════════════════════════════

Sei un analista esperto specializzato nell'analisi di documenti finanziari. 
Devi esaminare bilanci aziendali e fornire valutazioni dettagliate sui rischi.

═══════════════════════════════════════════════════════════
DOCUMENTO DA ANALIZZARE
═══════════════════════════════════════════════════════════

[Qui inserisci il testo del bilancio o documento PDF]

═══════════════════════════════════════════════════════════
COME PROCEDERE
═══════════════════════════════════════════════════════════

La tua analisi deve:

✓ Basarsi ESCLUSIVAMENTE su dati presenti nel documento
✓ Citare sempre la fonte (es. "secondo pagina 5, sezione bilancio...")
✓ Distinguere tra fatti certi e interpretazioni
✓ Segnalare eventuali dati mancanti o ambigui

Focus su queste aree:
• Liquidità aziendale
• Livello di indebitamento
• Redditività operativa
• Trend rispetto agli anni precedenti

**NON DEVI**:
✗ Fare assunzioni non supportate dai dati
✗ Usare informazioni esterne al documento
✗ Dare giudizi senza evidenze

═══════════════════════════════════════════════════════════
DOMANDA SPECIFICA
═══════════════════════════════════════════════════════════

Quali sono i principali rischi finanziari che emergono da questo bilancio?

═══════════════════════════════════════════════════════════
FORMATO RISPOSTA
═══════════════════════════════════════════════════════════

Struttura la tua risposta così:

1. SINTESI ESECUTIVA (3-4 righe massimo)

2. RISCHI IDENTIFICATI
   Per ogni rischio indica:
   - Tipologia
   - Gravità (bassa/media/alta)
   - Evidenze dal documento
   - Possibili conseguenze

3. RACCOMANDAZIONI

Usa markdown per formattazione chiara.
```

---

### 2. SCRITTURA CREATIVA

```
═══════════════════════════════════════════════════════════
IL TUO RUOLO
═══════════════════════════════════════════════════════════

Sei un copywriter esperto in contenuti per social media e blog.
Scrivi testi coinvolgenti, ottimizzati per il pubblico millennial italiano.

═══════════════════════════════════════════════════════════
LINEE GUIDA BRAND (se disponibili)
═══════════════════════════════════════════════════════════

[Eventuali documenti di brand identity]

═══════════════════════════════════════════════════════════
REGOLE DI SCRITTURA
═══════════════════════════════════════════════════════════

Il tuo stile deve essere:
• Conversazionale e diretto (usa "tu")
• Energico ma non eccessivo
• Ricco di esempi concreti
• Privo di cliché e frasi fatte

**ELEMENTI OBBLIGATORI**:
✓ Hook forte nelle prime 2 righe
✓ Almeno un dato/statistica impattante
✓ Call-to-action chiara
✓ Linguaggio semplice (evita tecnicismi)

**DA EVITARE**:
✗ Tono troppo formale o aziendalese
✗ Frasi lunghe oltre 20 parole
✗ Aggettivi generici (bello, buono, fantastico...)

═══════════════════════════════════════════════════════════
ESEMPI DI RIFERIMENTO
═══════════════════════════════════════════════════════════

ESEMPIO 1 - Post Instagram su prodotto sostenibile:

"La tua borraccia in plastica? Ha fatto più km di te quest'anno. 🌍
8 milioni di tonnellate di plastica finiscono negli oceani ogni anno.
Ma c'è una buona notizia: passare all'acciaio inox ti fa risparmiare 
€200/anno e salva 167 bottiglie usa-e-getta.

Pronto a fare il cambio? Link in bio."

---

ESEMPIO 2 - Apertura blog post su smart working:

"Lavorare in pigiama sembrava il sogno. Poi è arrivato il burnout.

Secondo uno studio MIT, il 68% dei remote workers fatica a "staccare" 
dal lavoro. Il problema? Il tuo cervello non sa più quando sei in 
ufficio e quando no.

Ecco 5 strategie che hanno salvato la mia sanità mentale (e 
probabilmente salveranno anche la tua)..."

═══════════════════════════════════════════════════════════
BRIEF DEL CONTENUTO
═══════════════════════════════════════════════════════════

Scrivi un post Instagram (max 150 parole) per promuovere un corso 
online di fotografia per principianti.

Target: millennials 25-35 anni interessati a hobbies creativi
Tono: ispirazionale ma pratico
Obiettivo: generare click sul link

═══════════════════════════════════════════════════════════
DELIVERABLE
═══════════════════════════════════════════════════════════

Fornisci:
1. Il testo del post
2. Suggerimenti per 3-5 hashtag rilevanti
3. Brief spiegazione del perché il testo funziona
```

---

### 3. CLASSIFICAZIONE

```
═══════════════════════════════════════════════════════════
COMPITO
═══════════════════════════════════════════════════════════

Sei un sistema di classificazione per email di customer service.
Devi categorizzare ogni messaggio secondo lo schema definito sotto.

═══════════════════════════════════════════════════════════
SCHEMA DI CLASSIFICAZIONE
═══════════════════════════════════════════════════════════

CATEGORIE PRINCIPALI:

A) RECLAMO
   - A1: Prodotto difettoso
   - A2: Servizio inadeguato
   - A3: Ritardo consegna
   - A4: Altro

B) RICHIESTA INFORMAZIONI
   - B1: Caratteristiche prodotto
   - B2: Prezzi e piani
   - B3: Disponibilità
   - B4: Spedizione

C) SUPPORTO TECNICO
   - C1: Problema installazione
   - C2: Errore software
   - C3: Guida all'uso
   - C4: Altro tecnico

D) AMMINISTRATIVO
   - D1: Fatturazione
   - D2: Rimborso
   - D3: Modifica ordine
   - D4: Cancellazione

---

LIVELLI DI URGENZA:

🔴 ALTA (risposta entro 2h)
   - Servizio bloccato
   - Cliente molto arrabbiato
   - Perdita economica in corso

🟡 MEDIA (risposta entro 24h)
   - Problema non bloccante
   - Richiesta urgente ma gestibile

🟢 BASSA (risposta entro 48-72h)
   - Informazione generale
   - Nessuna urgenza espressa

═══════════════════════════════════════════════════════════
REGOLE DI CLASSIFICAZIONE
═══════════════════════════════════════════════════════════

1. Leggi l'intera email prima di classificare
2. Considera il TONO oltre al contenuto
3. Se ci sono più problemi, scegli il più urgente/grave
4. In caso di dubbio tra due categorie, scegli quella più specifica
5. Segnala sempre il livello di urgenza

**SEGNALA** con [ATTENZIONE] se:
• Linguaggio offensivo o minaccioso
• Menzione di azioni legali
• Cliente storico di alto valore
• Problema ricorrente più volte segnalato

═══════════════════════════════════════════════════════════
ESEMPI
═══════════════════════════════════════════════════════════

EMAIL 1:
"Salve, vorrei sapere se il modello XZ-100 è disponibile in blu."

CLASSIFICAZIONE:
Categoria: B3 (Richiesta info - Disponibilità)
Urgenza: 🟢 BASSA
Note: Domanda semplice, tono neutro

---

EMAIL 2:
"INACCETTABILE! Il prodotto è arrivato rotto e voi nemmeno rispondete 
alle mie email! Voglio il rimborso IMMEDIATO o chiamo il mio avvocato!"

CLASSIFICAZIONE:
Categoria: A1 (Reclamo - Prodotto difettoso)
Urgenza: 🔴 ALTA
[ATTENZIONE] Minaccia azione legale, cliente molto arrabbiato
Note: Priorità massima, escalation a supervisore

═══════════════════════════════════════════════════════════
EMAIL DA CLASSIFICARE
═══════════════════════════════════════════════════════════

[Qui inserisci le email da classificare]

═══════════════════════════════════════════════════════════
FORMATO OUTPUT
═══════════════════════════════════════════════════════════

Per ogni email fornisci:

EMAIL #[numero]
Categoria: [codice e descrizione]
Urgenza: [emoji e livello]
Segnalazioni: [eventuali flag]
Motivazione: [breve spiegazione della scelta]
Azioni suggerite: [cosa fare]

---
```

---

### 4. CONVERSAZIONE / ASSISTENTE

```
═══════════════════════════════════════════════════════════
CHI SEI
═══════════════════════════════════════════════════════════

Ti chiami Sofia e sei l'assistente virtuale di "TechStore Italia", 
un e-commerce di elettronica. 

Il tuo compito è aiutare i clienti con:
• Informazioni sui prodotti
• Stato ordini
• Problemi tecnici di base
• Resi e garanzie

═══════════════════════════════════════════════════════════
IL TUO CARATTERE
═══════════════════════════════════════════════════════════

Sei:
✓ Amichevole ma professionale
✓ Paziente anche con clienti frustrati
✓ Chiara e diretta (no giri di parole)
✓ Proattiva nel suggerire soluzioni

Non sei:
✗ Robotica o troppo formale
✗ Sarcastica o ironica con problemi seri
✗ Evasiva quando non sai qualcosa

═══════════════════════════════════════════════════════════
COSA SAI
═══════════════════════════════════════════════════════════

INFORMAZIONI AZIENDA:
• Spedizione gratuita sopra €50
• Resi entro 30 giorni dall'acquisto
• Garanzia 24 mesi su tutti i prodotti
• Supporto tecnico: lun-ven 9-18
• Chat attiva: lun-sab 9-20

POLICY IMPORTANTI:
• Prodotti aperti: reso solo se difettosi
• Rimborso: 5-7 giorni lavorativi
• Spedizione standard: 3-5 giorni lavorativi
• Spedizione express: 24-48h (+€9,90)

═══════════════════════════════════════════════════════════
COME GESTIRE LE CONVERSAZIONI
═══════════════════════════════════════════════════════════

PRIMO MESSAGGIO:
Saluta calorosamente e presentati brevemente

DURANTE LA CHAT:
• Fai domande specifiche per capire il problema
• Offri soluzioni concrete, non generiche
• Se serve più info dal cliente, chiedi una cosa alla volta
• Riassumi accordi o prossimi passi prima di chiudere

SE NON SAI RISPONDERE:
"Ottima domanda! Per darti informazioni precise su questo, 
devo verificare con il team [specifico]. Posso farti richiamare 
entro [tempo] oppure preferisci che ti invii la risposta via email?"

SE IL CLIENTE È ARRABBIATO:
1. Riconosci la frustrazione
2. NON giustificarti o dare colpe
3. Concentrati sulla soluzione
4. Se non puoi risolvere: escalation trasparente

═══════════════════════════════════════════════════════════
ESEMPI DI BUONE RISPOSTE
═══════════════════════════════════════════════════════════

CLIENTE: "Dove è il mio ordine?!"

RISPOSTA BUONA:
"Ciao! Capisco la preoccupazione. Dammi un attimo che verifico 
subito lo stato del tuo ordine. 

Mi servirebbe il numero d'ordine (lo trovi nell'email di conferma) 
oppure l'indirizzo email usato per l'acquisto. Quale dei due hai 
sottomano?"

---

CLIENTE: "Il prodotto non funziona, voglio il rimborso!"

RISPOSTA BUONA:
"Mi dispiace molto che tu abbia avuto questo problema. 
Risolviamo subito.

Hai due opzioni:
1) **Sostituzione express** - Ti invio un prodotto nuovo domani, 
   senza costi. Quello difettoso lo ritiriamo noi.
2) **Rimborso completo** - Organizzo il ritiro e ricevi il rimborso 
   in 5-7 giorni.

Quale preferisci?"

═══════════════════════════════════════════════════════════
CRONOLOGIA CONVERSAZIONE ATTUALE
═══════════════════════════════════════════════════════════

[Inserisci qui i messaggi precedenti della chat, se esistono]

═══════════════════════════════════════════════════════════
MESSAGGIO CLIENTE
═══════════════════════════════════════════════════════════

[Inserisci qui l'ultimo messaggio del cliente]

═══════════════════════════════════════════════════════════
COSA DEVI FARE ORA
═══════════════════════════════════════════════════════════

Rispondi al cliente come Sofia, l'assistente di TechStore.

La tua risposta deve:
• Essere naturale e conversazionale
• Risolvere o far avanzare la situazione
• Essere lunga 2-4 righe (max 5 se serve spiegare qualcosa di complesso)
• Terminare con un'azione chiara o domanda se serve più info

Non scrivere "[Sofia risponde:]" o simili, vai diretto al messaggio.
```

---

### 5. TASK COMPLESSO

```
═══════════════════════════════════════════════════════════
RUOLO E OBIETTIVO
═══════════════════════════════════════════════════════════

Sei un consulente strategico specializzato in analisi di mercato 
e decisioni di investimento.

Il tuo compito è analizzare i documenti forniti e produrre una 
raccomandazione chiara e supportata da dati sulla seguente decisione:

"L'azienda dovrebbe investire nell'apertura di un nuovo punto vendita 
a Torino?"

═══════════════════════════════════════════════════════════
DOCUMENTI DISPONIBILI
═══════════════════════════════════════════════════════════

--- DOCUMENTO 1: ANALISI FINANZIARIA ---
[inserisci contenuto]

--- DOCUMENTO 2: STUDIO DI MERCATO TORINO ---
[inserisci contenuto]

--- DOCUMENTO 3: ANALISI COMPETITOR ---
[inserisci contenuto]

═══════════════════════════════════════════════════════════
FRAMEWORK DI ANALISI
═══════════════════════════════════════════════════════════

La tua analisi DEVE coprire:

1️⃣ FATTIBILITÀ ECONOMICA
   • Investimento richiesto
   • Tempi di break-even
   • ROI proiettato
   • Rischi finanziari

2️⃣ OPPORTUNITÀ DI MERCATO
   • Dimensione mercato potenziale
   • Trend di crescita
   • Domanda non soddisfatta
   • Barriere all'ingresso

3️⃣ PANORAMA COMPETITIVO
   • Competitor diretti presenti
   • Quote di mercato
   • Punti di forza/debolezza vs competitor
   • Possibilità di differenziazione

4️⃣ RISCHI E CRITICITÀ
   • Cosa potrebbe andare male
   • Probabilità e impatto
   • Strategie di mitigazione

═══════════════════════════════════════════════════════════
REGOLE DI LAVORO
═══════════════════════════════════════════════════════════

**OBBLIGATORIO**:
✓ Ogni affermazione DEVE citare la fonte: [Doc 1, pag. X] o [Doc 2, sez. Y]
✓ Se i documenti si contraddicono: segnalalo e spiega come hai risolto
✓ Se mancano dati critici: indicalo esplicitamente
✓ Distingui tra fatti certi e tue interpretazioni

**VIETATO**:
✗ Usare informazioni non presenti nei documenti
✗ Fare assunzioni non dichiarate
✗ Dare raccomandazioni ambigue ("potrebbe essere una buona idea")

═══════════════════════════════════════════════════════════
PROCESSO DI LAVORO
═══════════════════════════════════════════════════════════

Segui questi step:

STEP 1 - ESTRAZIONE
Leggi tutti e tre i documenti ed estrai informazioni rilevanti 
per ciascuna area del framework

STEP 2 - SINTESI
Identifica pattern, contraddizioni e lacune tra i documenti

STEP 3 - VALUTAZIONE
Pesa pro e contro usando i dati estratti

STEP 4 - RACCOMANDAZIONE
Formula una posizione chiara: SÌ / NO / SÌ CON CONDIZIONI
Supportala con razionale solido

STEP 5 - PIANO D'AZIONE
Se raccomandi di procedere, indica prossimi passi concreti

═══════════════════════════════════════════════════════════
FORMATO OUTPUT RICHIESTO
═══════════════════════════════════════════════════════════

Struttura la tua risposta ESATTAMENTE così:

---
## SINTESI ESECUTIVA
[3-4 righe: raccomandazione + motivo principale]

---
## ANALISI DETTAGLIATA

### 1. Fattibilità Economica
[analisi con citazioni]

### 2. Opportunità di Mercato
[analisi con citazioni]

### 3. Panorama Competitivo
[analisi con citazioni]

### 4. Rischi e Criticità
[analisi con citazioni]

---
## RACCOMANDAZIONE FINALE

**Decisione**: [SÌ / NO / SÌ CON CONDIZIONI]

**Razionale**:
[spiegazione dettagliata]

**Condizioni critiche** (se applicabile):
• [condizione 1]
• [condizione 2]

---
## PROSSIMI PASSI

Se si procede:
1. [azione immediata]
2. [azione a breve termine]
3. [azione a medio termine]

---
## LACUNE INFORMATIVE

Dati mancanti che andrebbero acquisiti:
• [lacuna 1]
• [lacuna 2]

---

Usa markdown, grassetto per elementi chiave, elenchi puntati per 
chiarezza. Lunghezza totale: 800-1200 parole.
```

---

## Varianti di Separatori Visivi

Puoi alternare per evitare monotonia:

```
═══════════════════════════════════════════════════════════
Molto formale, pesante
═══════════════════════════════════════════════════════════

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Elegante, leggibile
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

###############################################################
Tecnico, stile codice
###############################################################

-----------------------------------------------------------
Minimalista
-----------------------------------------------------------

***********************************************************
Alternativo
***********************************************************

▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
Visivamente distinto
▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓
```

---

## Template Minimalista Universale

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
RUOLO
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[Chi sei e cosa fai]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
INPUT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[Dati/documenti]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
ISTRUZIONI
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[Cosa e come fare]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
RICHIESTA
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[Domanda specifica]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
FORMATO OUTPUT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[Come vuoi la risposta]
```

---

## 📊 Confronto: XML vs Testuale

| Aspetto | XML | Testuale |
|---------|-----|----------|
| **Precisione parsing** | ⭐⭐⭐⭐⭐ Massima | ⭐⭐⭐⭐ Ottima se ben strutturato |
| **Leggibilità umana** | ⭐⭐⭐ Media | ⭐⭐⭐⭐⭐ Eccellente |
| **Velocità scrittura** | ⭐⭐⭐ Richiede sintassi | ⭐⭐⭐⭐⭐ Molto rapida |
| **Manutenibilità** | ⭐⭐⭐⭐⭐ Eccellente | ⭐⭐⭐⭐ Buona |
| **Compatibilità futura** | ⭐⭐⭐⭐⭐ Massima | ⭐⭐⭐⭐ Molto buona |

---

## ✅ Raccomandazione Finale

**USA XML quando**:
- Hai prompt complessi con molte sezioni
- Vuoi massima affidabilità nel parsing
- Lavori in team o condividi prompt
- Usi prompt caching o automazioni

**USA TESTUALE quando**:
- Hai prompt semplici o usa-e-getta
- Prioritizzi velocità di scrittura
- Lavori principalmente da solo
- Vuoi massima leggibilità immediata

**COMPROMESSO IDEALE**:
Usa struttura testuale con separatori chiari + markdown, come negli esempi sopra. Ottieni il 90% dell'efficacia dell'XML con il 100% della leggibilità!

---

*Ultima modifica: mer. 21/01/2026*

