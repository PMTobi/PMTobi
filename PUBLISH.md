# So geht dein neues GitHub-Profil live

Ein GitHub-Profil zeigt oben die README aus einem Repo, das **exakt so heißt wie dein Username**:
`PMTobi/PMTobi`. Das Repo gibt es noch nicht — in 2 Minuten ist es live.

## Schritt 1 — leeres Repo anlegen (einmalig, im Browser)
1. Öffne **https://github.com/new**
2. Repository name: **`PMTobi`** (GitHub zeigt dann „✨ You found a secret!" — genau richtig)
3. **Public** auswählen
4. **KEINEN** Haken bei „Add a README" (bleibt leer, wir pushen gleich)
5. **Create repository**

## Schritt 2 — Inhalt hochladen
Dieses Repo liegt fertig committet in `C:\Users\tobia\Desktop\PMTobi`. Push per:

```bash
cd C:\Users\tobia\Desktop\PMTobi
git push -u origin main
```

(Sag mir Bescheid, sobald Schritt 1 erledigt ist — dann pushe ich für dich.)

## Schritt 3 — die 🐍 Snake-Animation aktivieren (optional, fancy)
1. Im neuen Repo → **Settings → Actions → General** → „Allow all actions" sicherstellen.
2. Tab **Actions** → Workflow „🐍 Generate Contribution Snake" → **Run workflow**.
   (Läuft danach automatisch alle 12 h.) Er baut die Snake-SVGs auf den Branch `output`,
   die README zeigt sie automatisch. Bis zum ersten Lauf ist der Snake-Bereich leer.

## Hinweise
- Die Stats-/Streak-/Trophäen-Karten füllen sich mit deiner echten GitHub-Aktivität. Viel davon
  liegt in privaten Repos — mit `count_private=true` zählen private Commits, sobald du (optional)
  eine eigene Instanz oder das GitHub-eigene Rendering nutzt. Öffentlich sichtbar bleibt, was du
  freigibst.
- Falls eine Karte mal leer wirkt: die kostenlosen Community-Dienste (github-readme-stats & Co.)
  werden gelegentlich kurz rate-limited — das erholt sich von selbst.
