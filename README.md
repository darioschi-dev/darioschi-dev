# 👋 Ciao, sono Dario Schiavano

IoT & Full Stack Developer | Embedded Systems | Backend Services | AI Tooling

Sviluppo soluzioni integrate che combinano **embedded systems**, **IoT**, **backend services** e **automazione con agenti AI**. Dopo anni su MES e IoT industriale, il baricentro si è spostato verso piattaforme operative per il monitoraggio di impianti, app offline-first per il campo e strumenti che rendono ripetibile il lavoro con gli agenti AI.

---

## 🎯 Su cosa ho lavorato

Gran parte del lavoro vive in repository privati: qui ne descrivo l'obiettivo e le scelte tecniche, senza codice né dati.

### 🏭 Software per l'industria e IoT industriale

Sviluppo full stack di applicazioni per la produzione manifatturiera: backend **Symfony/PHP**, frontend **Angular** con test end-to-end, rilasci containerizzati con **Docker**, integrazione con sistemi gestionali esterni tramite API REST.

Sul fronte IoT, un **middleware universale per l'acquisizione dati industriale**: architettura a driver intercambiabili in Node.js/TypeScript che espone un'unica interfaccia verso macchinari e PLC di produttori diversi, con supporto ai protocolli industriali in uso (**Modbus**, **OPC-UA** e altri), lettura e scrittura normalizzate e simulazione dei dispositivi per i test. A corredo, firmware su **Raspberry Pi** per l'acquisizione sul campo.

### 📡 Piattaforme operative per impianti fotovoltaici

Backend **Symfony** e collector **Python** che centralizzano il monitoraggio di impianti oggi sparsi su più portali vendor: ingest di allarmi e snapshot, normalizzazione, gestione di eventi, casi operativi e ticket verso i vendor, contratti e manutenzioni, notifiche su Slack. Accanto alla piattaforma, registri operativi di dominio (manutenzioni, ricambi, incentivi, colonnine di ricarica) allineati al portale.

### 📱 App offline-first per operatori di campo

App **Flutter** per tecnici sul campo con architettura offline-first, affiancata da un backend gestionale e dalla documentazione dell'infrastruttura IT. Attenzione particolare a sincronizzazione, tag fisici (QR/NFC) che aprono l'azione giusta nell'app e decisioni di architettura tracciate come ADR.

### 🤖 Agenti AI e tooling per il lavoro quotidiano

Il filone più ampio degli ultimi mesi: rendere il lavoro con gli agenti AI **ripetibile, governato e sicuro**.

- **agent-toolkit** — control plane per connector, server MCP, skill e profili, con CLI di bootstrap e verifica (doctor) per avere lo stesso ambiente su macOS e Ubuntu; routing dei modelli, regole comuni e registro di lavoro condiviso tra agenti.
- **Connettori MCP** per Google Tasks, Passbolt (sola lettura) ed export ChatGPT: CLI, libreria Python e server MCP sullo stesso codice, gestiti con `uv`.
- **JARVIS** — assistente personale privato: quick capture di pensieri e arricchimento con LLM locale, API FastAPI e PWA.

### 🏠 Self-hosting su Raspberry Pi

Applicazioni personali in produzione su Raspberry Pi, esposte con **Cloudflare Tunnel** senza aprire porte sul router:

- **Ledger Home** — PWA per i conti familiari con import, categorie, dashboard ed export Excel.
- **StudyOS** — piattaforma di studio con quiz a risposta multipla e ripetizione spaziata (SM-2), autenticazione, pannello admin e banche dati su SQLite.
- **Personal Shopper AI** — ricerca parallela su più marketplace con ranking spiegato da LLM, con routing tra modelli cloud e fallback locale.
- **Cluster Raspberry** — dashboard di monitoraggio e deployment automatizzato dei nodi con **Ansible** e API Node.js.

### 🎙️ Strumenti desktop locali

**nispa-WhisperApp** — trascrizione automatica con Whisper in locale (GPU CUDA), editor sincronizzato audio/video e strumenti batch; frontend React, backend Flask.

---

## 🧭 Come lavoro

Parto dai vincoli del dominio e li metto per iscritto: decisioni di architettura documentate come ADR, test scritti prima del codice sulle funzionalità più grosse, segreti fuori dai repository e gestiti con un password manager, deploy ripetibili con Ansible o container. Preferisco strumenti semplici e self-hosted a soluzioni sovradimensionate, e verifico sul campo prima di dichiarare una cosa finita.

---

## 🏗️ Stack Tecnologico

**Microcontrollori & Hardware:**
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=Arduino)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=Espressif)

**Linguaggi & Frameworks:**
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=PHP)
![Symfony](https://img.shields.io/badge/Symfony-000000?style=for-the-badge&logo=Symfony)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=Node.js)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=TypeScript)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=Vue.js&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=Angular)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=Flutter&logoColor=white)

**Protocolli & Infrastrutture:**
![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge)
![Modbus](https://img.shields.io/badge/Modbus-4B5563?style=for-the-badge)
![OPC--UA](https://img.shields.io/badge/OPC--UA-0066CC?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=Docker)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=Ansible)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-A22846?style=for-the-badge&logo=RaspberryPi)
![Cloudflare](https://img.shields.io/badge/Cloudflare%20Tunnel-F38020?style=for-the-badge&logo=Cloudflare&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-000000?style=for-the-badge)

---

## 🔧 Progetti Pubblici

### 🌱 IoT & Embedded

#### 🚀 [bonsai-firmware](https://github.com/darioschi-dev/bonsai-firmware)
Sistema di irrigazione automatica per bonsai con **ESP32** e sensore di umidità.  
Progetto completo da firmware a sensori, ottimizzato per batterie e pannello solare.

![ESP32](https://img.shields.io/badge/MCU-ESP32-blue)
![Sensor](https://img.shields.io/badge/sensor-soil--moisture-green)
![MQTT](https://img.shields.io/badge/protocol-MQTT-yellow)
![OTA](https://img.shields.io/badge/OTA-enabled-success)

---

#### 🔐 [cassaforte-arduino](https://github.com/darioschi-dev/cassaforte-arduino)
Serratura elettronica intelligente basata su **Arduino Uno**.  
Tastierino 4x4, EEPROM per memorizzazione PIN, controllo solenoide e feedback acustico.

![Arduino](https://img.shields.io/badge/MCU-Arduino--Uno-blue)
![Keypad](https://img.shields.io/badge/input-4x4--keypad-9cf)
![Storage](https://img.shields.io/badge/storage-EEPROM-orange)
![Actuator](https://img.shields.io/badge/actuator-solenoid-success)

---

#### 📡 [opcua-rust-client](https://github.com/darioschi-dev/opcua-rust-client)
Client **OPC-UA** scritto in **Rust** per connessioni industriali.  
Prototipo per testing su broker MQTT e sistemi legacy.

![Rust](https://img.shields.io/badge/lang-Rust-orange)
![OPC--UA](https://img.shields.io/badge/protocol-OPC--UA-blueviolet)
![Industrial](https://img.shields.io/badge/use--case-Industrial-red)

---

### 🛠️ Backend & Services

#### 💬 [support-credit-system](https://github.com/darioschi-dev/support-credit-system)
Sistema di gestione supporto tecnico e pacchetti ore in **Docker**.  
Backend **Symfony**, integrazione **PayPal** e **Satispay**, dashboard per cliente e supporto.

![Docker](https://img.shields.io/badge/env-Docker-2496ED)
![Symfony](https://img.shields.io/badge/backend-Symfony-black)
![Payments](https://img.shields.io/badge/payments-PayPal%20%7C%20Satispay-red)
![PHP](https://img.shields.io/badge/lang-PHP-777BB4)

---

### 🤖 Bots & Tools

#### 🔍 [telegram-search-bot](https://github.com/darioschi-dev/telegram-search-bot)
Bot **Telegram** per ricerche avanzate in canali pubblici.  
Automazione e indicizzazione di contenuti.

![Telegram](https://img.shields.io/badge/platform-Telegram-0088cc)
![Python](https://img.shields.io/badge/lang-Python-3776AB)
![Bot](https://img.shields.io/badge/type-Bot%20API-yellow)

---

## 📫 Contatti

- 📧 Email: [dario.schiavano@gmail.com](mailto:dario.schiavano@gmail.com)
- 💼 LinkedIn: [linkedin.com/in/darioschiavano](https://www.linkedin.com/in/darioschiavano/)
- 🧑‍💻 GitHub: [github.com/darioschi-dev](https://github.com/darioschi-dev)

---

🪪 **Licenza**: MIT  
> I progetti pubblici elencati sono open source e liberamente riutilizzabili.

![Made with ❤️ by Dario Schiavano](https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F%20by%20Dario%20Schiavano-blue)

