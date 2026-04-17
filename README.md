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
Persone malinconiche, chi ha perso qualcuno di caro o chi vorrebbe rivivere viaggi ed emozioni importanti. Il target include anche utenti interessati a tecnologie innovative che uniscono emozione e memoria, oltre a professionisti del settore psicologico per percorsi di reminiscenza.

---

# Tagline:
"Rivivi i tuoi ricordi, oltre il tempo."

---

# Tecnologie Utilizzate:
- Frontend Mobile (App di gestione)
- Intelligenza Artificiale (Ricostruzione 3D)
- Realtà Virtuale (VR) e Aumentata (AR)
- Cloud Storage (Archivio media personali)
- Sistema di pagamenti (Gestione abbonamenti Premium)

---

# Implementazione Grafica:
Puoi visualizzare il prototipo interattivo dell'applicazione al seguente link:
[https://re-memory-lane.lovable.app](https://re-memory-lane.lovable.app)

---

## <span style="background:#E6F1FB;color:#0C447C;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Funzionali</span> &nbsp; 
> Funzionalità offerte agli utenti

- Registrazione di singoli utenti e creazione profilo personale
- Caricamento di foto, video e messaggi vocali dalla galleria dello smartphone
- Elaborazione tramite AI per la creazione di ambienti 3D realistici
- Interazione in ambiente VR (parlare, scherzare e muoversi nel ricordo)
- Visualizzazione catalogo visori VR disponibili e collegamento all'acquisto
- Salvataggio dei media nella galleria dedicata dell'applicazione
- Sottoscrizione di abbonamenti mensili o annuali (Base o Premium)
- Possibilità di rivivere scenari storici e viaggi passati (es. Mykonos) per utenti Premium
- Collegamento e configurazione tecnica del visore VR alla piattaforma

## <span style="background:#EAF3DE;color:#27500A;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Non Funzionali</span> &nbsp; 
> Qualità, performance, usabilità

- **Realismo Percepito:** l'ambiente 3D deve garantire un alto livello di immersione
- **Limiti Legali:** il sistema deve operare nel rispetto della privacy e delle normative vigenti
- **Usabilità:** interfaccia intuitiva per utenti di ogni fascia d'età
- **Affidabilità:** gestione sicura dei pagamenti tramite sistema bancario
- **Sicurezza:** protezione crittografata dei ricordi personali caricati

## <span style="background:#EEEDFE;color:#3C3489;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Di Dominio</span> &nbsp; 
> Regole e vincoli del contesto

- L'esperienza immersiva richiede necessariamente l'utilizzo di visori VR/AR
- La qualità della ricostruzione dipende dalla risoluzione dei media forniti
- L'accesso ai contenuti di viaggio e storici è vincolato al modello di abbonamento

---

# WBS
<img width="1612" height="248" alt="image" src="https://github.com/user-attachments/assets/56193df2-a4ba-440c-a3bb-c9d13f68a621" />


---

# gantt
<img width="1591" height="293" alt="image" src="https://github.com/user-attachments/assets/10352c49-baab-4922-af94-ed456801db3b" />


---

# Competitors:
Analisi comparativa basata sulle feature chiave di ReMemory rispetto ai leader di mercato:

| Feature | Importanza | ReMemory | Oculus (Meta) | Google Photos | Rendever |
| :--- | :---: | :---: | :---: | :---: | :---: |
| Ricostruzione 3D da media personali | **Alta** | ✅ | ❌ | ❌ | ❌ |
| Integrazione IA per ambienti 3D | **Alta** | ✅ | ❌ | ❌ | ⚠️ |
| Interazione con ricordi/persone | **Alta** | ✅ | ⚠️ | ❌ | ⚠️ |
| Focus su memoria e legami affettivi | **Media** | ✅ | ❌ | ⚠️ | ✅ |
| Abbonamento per esperienze extra | **Alta** | ✅ | ⚠️ | ❌ | ✅ |

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
