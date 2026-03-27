# Titolo: 
### ReMemory

---

# Descrizione: 
ReMemory è una piattaforma innovativa che permette di ricostruire e rivivere esperienze passate combinando intelligenza artificiale, Realtà Aumentata (AR) e Realtà Virtuale (VR). L’applicazione permette agli utenti di caricare ricordi personali sotto forma di foto, video e messaggi vocali. Grazie a un'IA avanzata, questi contenuti vengono elaborati per creare ambienti 3D realistici. 

Attraverso l'utilizzo di un visore VR, l'utente può immergersi in questi spazi per interagire con persone care, magari scomparse, o con vecchi amici, potendo parlare, scherzare e muoversi all'interno del ricordo. Oltre alla dimensione affettiva, ReMemory offre la possibilità di rivivere scenari storici, viaggi ed escursioni (come una serata a Mykonos) permettendo di provare nuovamente le stesse emozioni "come se fosse la prima volta". Il sistema si basa su un modello di abbonamento flessibile che sblocca diverse profondità di esperienza.

---

# Problema: 
Il progetto nasce per rispondere al bisogno emotivo di chi vive la malinconia o il lutto, offrendo un modo per colmare il vuoto lasciato dalla perdita di una persona cara. Molto spesso i ricordi digitali (foto e video) rimangono statici e frammentati all'interno di smartphone o PC. ReMemory risolve questa staticità trasformando media bidimensionali in esperienze immersive, aiutando chi desidera ripercorrere momenti significativi della propria vita o viaggi indimenticabili che non può più permettersi di rifare fisicamente.

---

# Target: 
Società e singoli utenti. Nello specifico: persone che hanno subito un lutto, nostalgici che vogliono rivivere viaggi, o utenti interessati alle potenzialità della VR/AR applicata alla memoria personale.

---

# Tagline:
"Rivivi i tuoi ricordi, oltre il tempo."

---

# Tecnologie Utilizzate:
Frontend Mobile (App di gestione).  
Intelligenza Artificiale (Ricostruzione 3D).  
Realtà Virtuale (VR) e Aumentata (AR).  
Cloud Storage (Archivio media).  
Sistema di pagamenti (Abbonamenti).  

---

# Requisiti – ReMemory
[![Requisiti](https://img.shields.io/badge/Requisiti-limegreen?style=for-the-badge&logo=googledocs&logoColor=white)](URL_TUO_DOCUMENTO)

## <span style="background:#E6F1FB;color:#0C447C;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Funzionali</span> &nbsp; 
> Funzionalità offerte agli utenti

- Registrazione di singoli utenti e creazione profilo personale
- Caricamento di foto, video e messaggi vocali dalla galleria dello smartphone
- Elaborazione tramite AI per la creazione di ambienti 3D realistici
- Interazione in ambiente VR (parlare, scherzare e muoversi nel ricordo)
- Visualizzazione catalogo visori VR disponibili e collegamento all'acquisto
- Gestione della galleria personale all'interno dell'app
- Sottoscrizione di abbonamenti mensili o annuali (Base o Premium)
- Accesso a scenari extra (viaggi, eventi storici) per utenti Premium
- Collegamento e configurazione del visore VR alla piattaforma

## <span style="background:#EAF3DE;color:#27500A;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Non Funzionali</span> &nbsp; 
> Qualità, performance, usabilità

- **Realismo:** elevata qualità percepita degli ambienti 3D generati
- **Usabilità:** interfaccia semplice per il caricamento dei contenuti multimediali
- **Sicurezza:** protezione dei dati personali e dei media caricati
- **Legalità:** rispetto delle normative sulla privacy e limiti etici nell'interazione
- **Portabilità:** compatibilità con i principali modelli di visori VR sul mercato

## <span style="background:#EEEDFE;color:#3C3489;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Di Dominio</span> &nbsp; 
> Regole e vincoli del contesto

- L'esperienza immersiva richiede necessariamente l'uso di un visore VR/AR
- Il contenuto 3D dipende strettamente dalla qualità dei media (foto/audio) caricati
- L'accesso alle esperienze di viaggio (es. Mykonos) è vincolato al piano Premium
- L'intelligenza artificiale deve operare entro i limiti della legalità vigente

---

# Competitors:
Il mercato della "Reminiscenza VR" è in crescita. ReMemory si differenzia per l'approccio "Consumer-Ready":
- **Oculus/Meta:** Focus su social e gaming, meno sulla memoria personale.
- **Google Photos:** Ottimo archivio, ma manca totalmente la componente immersiva 3D.
- **Rendever/MyndVR:** Focalizzati su cliniche e anziani, mentre ReMemory è per l'utente privato.

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
