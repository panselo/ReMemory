# Titolo: 
### ReMemory

---

# Descrizione: 
[cite_start]ReMemory è una piattaforma innovativa che permette di ricostruire e rivivere esperienze passate combinando intelligenza artificiale, Realtà Aumentata (AR) e Realtà Virtuale (VR)[cite: 2]. [cite_start]L’applicazione permette agli utenti di caricare ricordi personali sotto forma di foto, video e messaggi vocali. [cite_start]Grazie a un'IA avanzata, questi contenuti vengono elaborati per creare ambienti 3D realistici. 

[cite_start]Attraverso l'utilizzo di un visore VR, l'utente può immergersi in questi spazi per interagire con persone care, magari scomparse, o con vecchi amici, potendo parlare, scherzare e muoversi all'interno del ricordo. [cite_start]Oltre alla dimensione affettiva, ReMemory offre la possibilità di rivivere scenari storici, viaggi ed escursioni (come una serata a Mykonos) permettendo di provare nuovamente le stesse emozioni "come se fosse la prima volta". [cite_start]Il sistema si basa su un modello di abbonamento flessibile che sblocca diverse profondità di esperienza.

---

# Problema: 
[cite_start]Il progetto nasce per rispondere al bisogno emotivo di chi vive la malinconia o il lutto, offrendo un modo per colmare il vuoto lasciato dalla perdita di una persona cara. Molto spesso i ricordi digitali (foto e video) rimangono statici e frammentati all'interno di smartphone o PC. [cite_start]ReMemory risolve questa staticità trasformando media bidimensionali in esperienze immersive, aiutando chi desidera ripercorrere momenti significativi della propria vita o viaggi indimenticabili[cite: 10, 11].

---

# Target: 
[cite_start]Persone malinconiche, chi ha perso qualcuno di caro o chi vorrebbe rivivere viaggi ed emozioni importanti. [cite_start]Il target include anche utenti interessati a tecnologie innovative che uniscono emozione e memoria.

---

# Tagline:
"Rivivi i tuoi ricordi, oltre il tempo."

---

# Tecnologie Utilizzate:
Frontend Mobile (App di gestione).  
[cite_start]Intelligenza Artificiale (Ricostruzione 3D).  
[cite_start]Realtà Virtuale (VR) e Aumentata (AR).  
Cloud Storage (Archivio media).  
[cite_start]Sistema di pagamenti (Abbonamenti Premium).  

---

# Requisiti – ReMemory
[![Requisiti](https://img.shields.io/badge/Requisiti-limegreen?style=for-the-badge&logo=googledocs&logoColor=white)](https://docs.google.com/document/d/1xWKr9zPorj-nm3MxhnGaykbhv_UhUK95PsWAqKO3TZ0/edit?usp=sharing)

## <span style="background:#E6F1FB;color:#0C447C;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Funzionali</span> &nbsp; 
> Funzionalità offerte agli utenti

- Registrazione di singoli utenti e creazione profilo personale
- Caricamento di foto, video e messaggi vocali dalla galleria dello smartphone o dell'app
- [cite_start]Elaborazione tramite AI per la creazione di ambienti 3D realistici 
- [cite_start]Interazione in ambiente VR (parlare, scherzare e muoversi nel ricordo) 
- Visualizzazione catalogo visori VR disponibili e collegamento all'acquisto
- Salvataggio dei media nella galleria dedicata dell'applicazione
- Sottoscrizione di abbonamenti mensili o annuali (Base o Premium)
- [cite_start]Possibilità di rivivere scenari storici e viaggi passati (es. Mykonos) per utenti Premium 
- Collegamento e configurazione tecnica del visore VR

## <span style="background:#EAF3DE;color:#27500A;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Non Funzionali</span> &nbsp; 
> Qualità, performance, usabilità

- [cite_start]**Realismo Percepito:** l'ambiente 3D deve garantire un alto livello di immersione [cite: 7]
- [cite_start]**Limiti Legali:** il sistema deve operare nel rispetto della privacy e delle normative vigenti [cite: 7]
- [cite_start]**Usabilità:** interfaccia intuitiva per utenti di ogni fascia d'età [cite: 7]
- **Affidabilità:** gestione sicura dei pagamenti tramite sistema bancario

## <span style="background:#EEEDFE;color:#3C3489;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Di Dominio</span> &nbsp; 
> Regole e vincoli del contesto

- [cite_start]L'esperienza richiede l'utilizzo di tecnologie VR/AR e Intelligenza Artificiale [cite: 7]
- [cite_start]La fruizione immersiva è vincolata all'uso di un visore VR 
- [cite_start]La creazione di società o l'accesso a contenuti extra è vincolata a un modello di abbonamento [cite: 7]

---

# Competitors:
[cite_start]Analisi comparativa basata sulle feature chiave di ReMemory rispetto ai leader di mercato:

| Feature | Importance | ReMemory | Meta (Oculus) | Google Photos | Rendever |
| :--- | :---: | :---: | :---: | :---: | :---: |
| Ricostruzione 3D esperienze personali | **High** | ✅ | ❌ | ❌ | ❌ |
| Integrazione AI per ambienti realistici | **High** | ✅ | ❌ | ❌ | ⚠️ |
| Interazione con ricordi/persone | **High** | ✅ | ⚠️ | ❌ | ⚠️ |
| Focus su legami affettivi | **Moderate** | ✅ | ❌ | ⚠️ | ✅ |
| Abbonamento per esperienze extra | **High** | ✅ | ⚠️ | ❌ | ✅ |

---

# Use Case Diagram:
```mermaid
graph LR
    Visitor((Utente Visitatore))
    User((Utente Registrato))
    Bank((Sistema Bancario))
    Admin((Amministrazione))

    Visitor --> Reg(Registrazione)
    User --> Login(Login)
    User --> Piano(Gestisci il tuo piano)
    Bank --> Piano
    User --> Salva(Salva foto in galleria app)
    User --> Visita(Visita catalogo visori)
    Admin --> Visita
    
    Login -.->|include| Link(Collegamento Visore)
    Link -.->|include| Ins1(Carica da telefono)
    Link -.->|include| Ins2(Carica da App)
    Ins1 -.->|include| Rivivi((RIVIVI))
    Ins2 -.->|include| Rivivi
