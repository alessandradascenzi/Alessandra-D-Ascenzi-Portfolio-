Automazione Recruiting LinkedIn con n8n

Questo workflow automatizzato permette di estrarre e valutare i contatti da LinkedIn integrando Google Search, modelli LLM (Gemini) e Airtable.

 Come funziona
1. **Trigger Giornaliero:** Avvia la ricerca ogni mattina alle 9:00.
2. **Ricerca Google Custom Search:** Esegue la ricerca mirata per trovare profili LinkedIn in linea con le keyword.
3. **LLM 1 (Gemini):** Analizza i risultati grezzi ed estrae solo i profili validi in formato JSON.
4. **Divisione & Scoring:** Processa i profili uno ad uno e utilizza **LLM 2 (Gemini)** per assegnare un punteggio di pertinenza da 0 a 5.
5. **Airtable:** Unisce le informazioni ed inserisce i dati completi nel database.

 Requisiti
- Un'istanza n8n funzionante.
- Chiave API Google Custom Search e ID Motore di Ricerca.
- Chiave API Google Gemini (PaLM).
- Personal Access Token di Airtable con Base e Tabella configurate.
