# maakeen.site — Installatiegids

## Wat zit er in deze map?

```
index.html      → De landingspagina
builder.html    → De AI website builder
api/generate.js → De backend (verbergt je API-sleutel)
vercel.json     → Vercel configuratie
```

---

## Stap 1 — Maak een Anthropic account

1. Ga naar https://console.anthropic.com
2. Maak een account aan
3. Ga naar "API Keys" en klik op "Create Key"
4. Kopieer de sleutel (begint met `sk-ant-...`)
5. Stort €5–10 op je account (genoeg voor honderden websites)

---

## Stap 2 — Maak een Vercel account

1. Ga naar https://vercel.com
2. Klik op "Sign Up" en maak een gratis account
3. Je kunt inloggen met GitHub, GitLab of e-mail

---

## Stap 3 — Deploy naar Vercel

### Optie A: Via de website (makkelijkst)

1. Ga naar https://vercel.com/new
2. Klik op "Browse" of sleep deze hele map naar het uploadvenster
3. Klik op "Deploy"
4. Wacht ~30 seconden

### Optie B: Via de terminal

```bash
npm install -g vercel
cd /pad/naar/deze/map
vercel
```

---

## Stap 4 — Voeg je API-sleutel toe

Dit is de **belangrijkste stap** — zonder dit werkt de AI niet.

1. Ga naar je project op vercel.com
2. Klik op "Settings" → "Environment Variables"
3. Voeg toe:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** jouw sleutel (bijv. `sk-ant-api03-...`)
4. Klik op "Save"
5. Ga naar "Deployments" en klik op "Redeploy"

---

## Klaar! 🎉

Je site staat nu live op een URL zoals `mijnproject.vercel.app`

Wil je een eigen domeinnaam (bijv. `maakeen.site`)?
→ Koop een domein bij Transip of Hostnet (~€10/jaar)
→ Ga naar Vercel → Settings → Domains → voeg je domein toe

---

## Kosten

| Wat | Kosten |
|-----|--------|
| Vercel hosting | Gratis |
| Domeinnaam | ~€10/jaar (optioneel) |
| Per gegenereerde website | ~€0,05–0,15 |
| Per maand (100 gebruikers) | ~€5–15 |

---

## Vragen?

Maak het platform eerst live en test het. Succes!
