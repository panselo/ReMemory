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
Frontend Mobile.  
Intelligenza Artificiale.  
Realtà Virtuale (VR).  
Realtà Aumentata (AR).  
Cloud Storage.  

---

# Requisiti – ReMemory
[![Requisiti](https://img.shields.io/badge/Requisiti-limegreen?style=for-the-badge&logo=googledocs&logoColor=white)](https://docs.google.com/document/d/1xWKr9zPorj-nm3MxhnGaykbhv_UhUK95PsWAqKO3TZ0/edit?usp=sharing)

## <span style="background:#E6F1FB;color:#0C447C;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Funzionali</span> &nbsp; 
> Funzionalità offerte agli utenti

- Registrazione di singoli utenti con creazione di un'utenza personale
- Caricamento di foto, video e messaggi vocali dalla galleria dello smartphone
- Elaborazione del contenuto tramite AI per la creazione di ambienti 3D
- Interazione realistica in ambiente VR (parlare, scherzare, muoversi)
- Visualizzazione del catalogo visori compatibili e collegamento per l'acquisto
- Gestione della galleria personale per salvare i propri contenuti multimediali
- Sottoscrizione di abbonamento mensile o annuale (Base o Premium)
- Accesso a scenari extra (viaggi, eventi storici) per utenti Premium
- Collegamento tecnico del visore VR alla piattaforma

## <span style="background:#EAF3DE;color:#27500A;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Non Funzionali</span> &nbsp; 
> Qualità, performance, usabilità

- **Realismo:** elevata qualità percepita degli ambienti 3D ricostruiti
- **Usabilità:** interfaccia semplice e intuitiva per utenti di ogni età
- **Sicurezza:** gestione sicura dei dati personali e dei media caricati
- **Legalità:** rispetto dei limiti etici e legali nell'interazione virtuale
- **Affidabilità:** tracciamento preciso dei pagamenti degli abbonamenti

## <span style="background:#EEEDFE;color:#3C3489;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Di Dominio</span> &nbsp; 
> Regole e vincoli del contesto

- L'esperienza immersiva è vincolata all'utilizzo di un visore VR
- La qualità della ricostruzione dipende dai media forniti dall'utente
- L'accesso ai contenuti di viaggio è limitato al piano Premium
- Il sistema opera integrando tecnologie VR/AR e Intelligenza Artificiale

---

# Competitors:

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
