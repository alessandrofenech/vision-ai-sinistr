# 🛡️ Vision AI Sinistri

Assistente guidato per la gestione dei sinistri assicurativi, basato su Claude AI di Anthropic.

## Funzionalità

- Descrizione del sinistro tramite testo o dettatura vocale
- Analisi AI della copertura assicurativa
- Guida passo-passo su cosa fare
- Caricamento foto e video come allegati
- Riepilogo finale della pratica

## Come usare localmente

1. **Clona il repository**
   ```
   git clone https://github.com/TUO_USERNAME/vision-ai-sinistri.git
   cd vision-ai-sinistri
   ```

2. **Configura la chiave API**

   Crea il file `config.js` (già escluso da `.gitignore`):
   ```js
   window.APP_CONFIG = {
     ANTHROPIC_API_KEY: "la-tua-api-key"
   };
   ```
   Puoi ottenere la chiave su [console.anthropic.com](https://console.anthropic.com).

3. **Apri l'app**

   Apri `index.html` nel browser. Non serve nessun server.

## Deploy su GitHub Pages

1. Vai su **Settings → Pages**
2. Seleziona `Deploy from a branch → main`
3. Clicca **Save**

⚠️ **Importante:** su GitHub Pages il file `config.js` non viene caricato (è nel `.gitignore`).  
Per usare l'app online devi configurare un backend sicuro che non esponga la chiave API.

## Personalizzazione

- Modifica il `SYSTEM_PROMPT` in `index.html` per aggiornare la knowledge base delle polizze
- Cambia l'email di invio nel blocco "Riepilogo" con quella reale della tua agenzia

## Tecnologie

- React 18 (CDN)
- Babel Standalone
- Claude API (claude-sonnet-4-6)
- Web Speech API (dettatura vocale)

## Licenza

Uso privato — tutti i diritti riservati.
