# Titolo: 
### ReMemory

---

# Descrizione: 
ReMemory è una piattaforma innovativa che permette di ricostruire e rivivere esperienze passate combinando intelligenza artificiale, Realtà Aumentata (AR) e Realtà Virtuale (VR). L’applicazione permette agli utenti di caricare ricordi personali sotto forma di foto, video e messaggi vocali. Grazie a un'IA avanzata, questi contenuti vengono elaborati per creare ambienti 3D realistici. 

Attraverso l'utilizzo di un visore VR, l'utente può immergersi in questi spazi per interagire con persone care, magari scomparse, o con vecchi amici, potendo parlare, scherzare e muoversi all'interno del ricordo. Oltre alla dimensione affettiva, ReMemory offre la possibilità di rivivere scenari storici, viaggi ed escursioni (come una serata a Mykonos) permettendo di provare nuovamente le stesse emozioni "come se fosse la prima volta". Il sistema si basa su un modello di abbonamento flessibile che sblocca diverse profondità di esperienza.

---

# Problema: 
Il progetto nasce per rispondere al bisogno emotivo di chi vive la malinconia o il lutto, offrendo un modo per colmare il vuoto lasciato dalla perdita di una persona cara. Molto spesso i ricordi digitali (foto e video) rimangono statici e frammentati all'interno di smartphone o PC. ReMemory risolve questa staticità trasformando media bidimensionali in esperienze immersive, aiutando chi desidera ripercorrere momenti significativi della propria vita o viaggi indimenticabili.

---

# Target: 
Persone malinconiche, chi ha perso qualcuno di caro o chi vorrebbe rivivere viaggi ed emozioni importanti. Il target include anche utenti interessati a tecnologie innovative che uniscono emozione e memoria.

---

# Tagline:
"Rivivi i tuoi ricordi, oltre il tempo."

---

# Tecnologie Utilizzate:
- Frontend Mobile (App di gestione)
- Intelligenza Artificiale (Ricostruzione 3D)
- Realtà Virtuale (VR) e Aumentata (AR)
- Cloud Storage (Archivio media)
- Sistema di pagamenti (Abbonamenti Premium)

---

# Requisiti – ReMemory
[![Requisiti](https://img.shields.io/badge/Requisiti-limegreen?style=for-the-badge&logo=googledocs&logoColor=white)](URL_TUO_DOCUMENTO)

## <span style="background:#E6F1FB;color:#0C447C;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Funzionali</span> &nbsp; 
> Funzionalità offerte agli utenti

- Registrazione di singoli utenti e creazione profilo personale
- Caricamento di foto, video e messaggi vocali dalla galleria dello smartphone o dell'app
- Elaborazione tramite AI per la creazione di ambienti 3D realistici
- Interazione in ambiente VR (parlare, scherzare e muoversi nel ricordo)
- Visualizzazione catalogo visori VR disponibili e collegamento all'acquisto
- Salvataggio dei media nella galleria dedicata dell'applicazione
- Sottoscrizione di abbonamenti mensili o annuali (Base o Premium)
- Possibilità di rivivere scenari storici e viaggi passati (es. Mykonos) per utenti Premium
- Collegamento e configurazione tecnica del visore VR

## <span style="background:#EAF3DE;color:#27500A;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Non Funzionali</span> &nbsp; 
> Qualità, performance, usabilità

- **Realismo Percepito:** l'ambiente 3D deve garantire un alto livello di immersione
- **Limiti Legali:** il sistema deve operare nel rispetto della privacy e delle normative vigenti
- **Usabilità:** interfaccia intuitiva per utenti di ogni fascia d'età
- **Affidabilità:** gestione sicura dei pagamenti tramite sistema bancario

## <span style="background:#EEEDFE;color:#3C3489;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Di Dominio</span> &nbsp; 
> Regole e vincoli del contesto

- L'esperienza richiede l'utilizzo di tecnologie VR/AR e Intelligenza Artificiale
- La fruizione immersiva è vincolata all'uso di un visore VR
- La creazione di ambienti o l'accesso a contenuti extra è vincolata a un modello di abbonamento

---

# Competitors:
Analisi comparativa basata sulle feature chiave di ReMemory rispetto ai leader di mercato:

| Feature | Importanza | ReMemory | Oculus (Meta) | Google Photos | Rendever |
| :--- | :---: | :---: | :---: | :---: | :---: |
| Ricostruzione 3D da media personali | **Alta** | ✅ | ❌ | ❌ | ❌ |
| Integrazione IA per ambienti 3D | **Alta** | ✅ | ❌ | ❌ | ⚠️ |
| Interazione con persone/ricordi | **Alta** | ✅ | ⚠️ | ❌ | ⚠️ |
| Focus su memoria e legami affettivi | **Media** | ✅ | ❌ | ⚠️ | ✅ |
| Abbonamento per esperienze extra | **Alta** | ✅ | ⚠️ | ❌ | ✅ |
| Compatibilità diversi visori | **Media** | ✅ | ⚠️ | ❌ | ✅ |

---

# Use Case Diagram:
L'utente interagisce con il sistema attraverso diverse fasi: dalla registrazione al collegamento del visore fino alla fruizione dell'esperienza "Rivivi".

```mermaid
graph LR
    User((Utente Registrato))
    Visitatore((Utente Visitatore))
    Admin((Amministrazione))
    Banca((Sistema Bancario))

    Visitatore --> Reg(Registrazione)
    User --> Login(Login)
    User --> Piano(Gestisci il tuo piano)
    Banca --> Piano
    User --> Salva(Salva foto su galleria app)
    User --> Visita(Visita catalogo visori)
    Admin --> Visita
    
    Login -.->|include| Link(Collegamento Visore)
    Link -.->|include| Ins1(Inserisci foto/video da telefono)
    Link -.->|include| Ins2(Inserisci foto/video da app)
    Ins1 -.->|include| Rivivi((RIVIVI))
    Ins2 -.->|include| Rivivi




# WBS
    A[ReMemory Project] --> B[1.0 ANALISI E REQUISITI]
    A --> C[2.0 SVILUPPO IA E ASSET]
    A --> D[3.0 INTEGRAZIONE VR/AR]
    A --> E[4.0 BUSINESS E LANCIO]

    B --> B1[Definizione Requisiti Funzionali]
    B --> B2[Analisi Vincoli Legali e Privacy]
    B --> B3[User Case e Flussi Utente]

    C --> C1[Training Modello IA Ricostruzione 3D]
    C --> C2[Gestione Cloud Storage Media]
    C --> C3[Generazione Ambienti Realistici]

    D --> D1[Sviluppo Interfaccia App Mobile]
    D --> D2[Configurazione Collegamento Visore]
    D --> D3[Ottimizzazione Interazione 3D]

    E --> E1[Integrazione Sistema Abbonamenti]
    E --> E2[Catalogo Visori e Partnership]
    E --> E3[Pubblicazione Store]

---

# gantt
    title Cronoprogramma Sviluppo ReMemory
    dateFormat  YYYY-MM-DD
    axisFormat  W%W
    
    section Analisi
    Analisi Requisiti e Legale      :active, a1, 2026-01-01, 10d
    Design Diagrammi UML            : a2, after a1, 5d
    
    section Sviluppo IA
    Training Modelli 3D             : b1, 2026-01-15, 20d
    Integrazione Audio/Video        : b2, after b1, 10d
    
    section VR & App
    Sviluppo App Mobile             : c1, 2026-02-01, 25d
    Test Collegamento Visore        : c2, after c1, 10d
    
    section Business
    Setup Piani Premium             : d1, 2026-02-15, 7d
    Lancio e Marketing              : d2, after c2, 7d

---

# Implementazione: https://re-memory-lane.lovable.app
