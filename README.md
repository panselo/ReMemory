# Titolo: 
### ReMemory

---

# Descrizione: 
[cite_start]ReMemory è una piattaforma innovativa che permette di ricostruire e rivivere esperienze passate combinando intelligenza artificiale, Realtà Aumentata (AR) e Realtà Virtuale (VR)[cite: 2]. [cite_start]L’applicazione permette agli utenti di caricare ricordi personali sotto forma di foto, video e messaggi vocali. [cite_start]Grazie a un'IA avanzata, questi contenuti vengono elaborati per creare ambienti 3D realistici[cite: 4, 9]. 

[cite_start]Attraverso l'utilizzo di un visore VR, l'utente può immergersi in questi spazi per interagire con persone care, magari scomparse, o con vecchi amici, potendo parlare, scherzare e muoversi all'interno del ricordo. [cite_start]Oltre alla dimensione affettiva, ReMemory offre la possibilità di rivivere scenari storici, viaggi ed escursioni (come una serata a Mykonos) permettendo di provare nuovamente le stesse emozioni "come se fosse la prima volta". [cite_start]Il sistema si basa su un modello di abbonamento flessibile che sblocca diverse profondità di esperienza[cite: 5, 11].

---

# Problema: 
[cite_start]Il progetto nasce per rispondere al bisogno emotivo di chi vive la malinconia o il lutto, offrendo un modo per colmare il vuoto lasciato dalla perdita di una persona cara[cite: 10]. Molto spesso i ricordi digitali (foto e video) rimangono statici e frammentati all'interno di smartphone o PC. [cite_start]ReMemory risolve questa staticità trasformando media bidimensionali in esperienze immersive, aiutando chi desidera ripercorrere momenti significativi della propria vita o viaggi indimenticabili che non può più permettersi di rifare fisicamente[cite: 5, 10].

---

# Target: 
- [cite_start]**Persone in lutto:** chi desidera un ultimo contatto o un modo per mantenere vivo il legame con una persona cara[cite: 10].
- [cite_start]**Nostalgici e Viaggiatori:** chi vuole rivivere emozioni legate a luoghi ed eventi passati[cite: 10].
- [cite_start]**Utenti Tech-Enthusiast:** appassionati di VR/AR che cercano applicazioni pratiche ed emozionali della tecnologia[cite: 11].

---

# Tagline:
"Rivivi i tuoi ricordi, oltre il tempo."

---

# Tecnologie Utilizzate:
- [cite_start]**Intelligenza Artificiale:** Ricostruzione 3D e generazione ambienti[cite: 4, 9].
- [cite_start]**Realtà Virtuale (VR):** Per l'immersione totale tramite visore[cite: 4, 8].
- [cite_start]**Realtà Aumentata (AR):** Per l'integrazione dei ricordi nel mondo reale[cite: 2].
- **Cloud Storage:** Per l'archiviazione sicura dei media personali.

---

# Requisiti – ReMemory

## <span style="background:#E6F1FB;color:#0C447C;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Funzionali</span> &nbsp; 
> [cite_start]Cosa deve fare il sistema [cite: 7]

- **Registrazione e Login:** Gestione dell'utenza e del profilo personale.
- [cite_start]**Caricamento Media:** Inserimento di foto, video e messaggi vocali dalla galleria o dall'app[cite: 3, 4].
- [cite_start]**Generazione Ambiente 3D:** Elaborazione tramite AI dei contenuti caricati[cite: 4, 9].
- [cite_start]**Interazione VR:** Possibilità di parlare, scherzare e interagire con le persone nell'ambiente creato.
- [cite_start]**Gestione Abbonamenti:** Sottoscrizione di piani Base o Premium (mensili/annuali).
- **Catalogo Visori:** Consultazione e acquisto di visori compatibili tramite siti esterni.
- **Salvataggio Ricordi:** Archiviazione delle esperienze generate nella galleria personale dell'app.

## <span style="background:#EAF3DE;color:#27500A;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Non Funzionali</span> &nbsp; 
> [cite_start]Qualità e vincoli [cite: 7]

- [cite_start]**Realismo Percepito:** L'ambiente 3D deve essere sufficientemente realistico per garantire l'immersione.
- **Usabilità:** Interfaccia intuitiva per facilitare il caricamento dei file.
- [cite_start]**Limiti Legali:** Il sistema deve operare nei limiti della legalità (privacy e diritti d'immagine).
- [cite_start]**Compatibilità:** Supporto ai principali visori VR sul mercato[cite: 12].

## <span style="background:#EEEDFE;color:#3C3489;padding:3px 10px;border-radius:6px;font-size:13px;font-weight:500;">Di Dominio</span> &nbsp; 
> [cite_start]Contesto e regole del dominio [cite: 7]

- [cite_start]**Tecnologie Immersive:** Utilizzo obbligatorio di VR/AR per la fruizione[cite: 2].
- [cite_start]**Modello SaaS:** Accesso alle funzionalità tramite abbonamento premium.
- [cite_start]**Elaborazione AI:** L'ambiente è generato algoritmocamente partendo da input utente.

---

# Competitors:
Il mercato attuale presenta diverse soluzioni frammentate che ReMemory punta a unificare:
- [cite_start]**Oculus (Meta):** Focalizzato sul gaming e social VR, ma senza focus specifico sulla ricostruzione di ricordi personali[cite: 12].
- [cite_start]**Google Photos:** Gestione eccellente di media statici (foto/video), ma privo di immersività 3D[cite: 12].
- [cite_start]**Matterport:** Leader nella scansione 3D di ambienti reali, ma non focalizzato sui legami affettivi o ricordi personali[cite: 12].
- [cite_start]**MyndVR / Rendever:** Focalizzati sulla terapia della reminiscenza per anziani, simili ma meno orientati all'utente consumer generico[cite: 12].

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
