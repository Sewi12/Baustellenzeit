# Baustellenzeit – Cloud-Version

Diese Version kann auf iPhone, iPad und PC dieselben Daten verwenden.
Die Daten werden in Supabase gespeichert. IndexedDB/localStorage bleiben zusätzlich als lokaler Offline-Puffer erhalten.

## Einrichtung
1. Kostenloses Supabase-Projekt anlegen.
2. Im Supabase SQL Editor den Inhalt von `supabase-schema.sql` ausführen.
3. In Supabase die Project URL und den `anon/public` Key kopieren.
4. Im SQL Editor den Inhalt von `supabase-schema.sql` ausführen. Danach in `supabase-config.js` Project URL und Publishable Key eintragen:
   - `BAUSTELLENZEIT_SUPABASE_URL`
   - `BAUSTELLENZEIT_SUPABASE_ANON_KEY`
5. Alle Dateien auf GitHub Pages hochladen.
6. App öffnen und unter **Mehr → Cloud-Synchronisation** ein Konto erstellen.
7. Beim ersten Login fragt die App, ob vorhandene lokale Daten in die Cloud übernommen werden sollen.

WICHTIG: Niemals den `service_role` Key in die Website eintragen. Für die Browser-App ausschließlich den `anon/public` Key verwenden.
