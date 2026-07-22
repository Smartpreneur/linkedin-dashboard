# LinkedIn Analytics Dashboard

Ein kostenloses, privates Dashboard für deinen LinkedIn-Analytics-Export.
Zieh die XLSX-Datei rein und sieh sofort:

- **KPIs**: Impressions, erreichte Personen, Follower-Wachstum, Ø Engagement-Rate, aktive Monate
- **Reichweite & Wachstum pro Monat** — der Konsistenz-Check
- **Engagement-Rate pro Monat** — resoniert dein Content?
- **Top-Beiträge** sortierbar nach Impressions, Engagement und ER
- **Audience-Demografie** — passt deine Zielgruppe zu deinem Angebot?
- **Automatische Reflexions-Insights** aus deinen Zahlen

**🔒 Privacy first:** Alles läuft im Browser. Deine Daten werden nirgendwohin hochgeladen — es gibt kein Backend.

## So bekommst du deinen Export

1. LinkedIn → dein Profil → **Analytics** → *Beitragsimpressions*
2. Zeitraum auf **365 Tage** stellen
3. **Exportieren** → du bekommst `LinkedIn_AggregateAnalytics_….xlsx`
4. Datei ins Dashboard ziehen — fertig

Deutsche und englische Exporte werden unterstützt.

## Selbst hosten (Vercel)

Das Projekt ist eine einzige statische HTML-Seite — kein Build-Schritt.

```bash
git clone https://github.com/DEIN-USER/linkedin-dashboard
cd linkedin-dashboard
npx vercel        # oder: Repo bei vercel.com importieren
```

Alternativ lokal öffnen:

```bash
npx serve .       # wegen fetch() für die Demo-Daten nicht per file:// öffnen
```

## Struktur

| Datei | Zweck |
|---|---|
| `index.html` | Komplette App: Parsing (SheetJS), Charts (plain SVG), Insights |
| `demo-data.json` | Synthetische Beispieldaten für den „Demo ansehen"-Button |

## Lizenz

MIT — fork it, mach's zu deinem.
