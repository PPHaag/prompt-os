# 📥 Inbox

Dit is de capture-laag van Prompt OS. Alles wat je tegenkomt op X, LinkedIn, blogs of elders en interessant lijkt, gooit je hier in — zonder nadenken over structuur, tags of kwaliteit.

> Snel opslaan nu. Beoordelen later.

---

## 🗂️ Submappen

| Map | Gebruik |
|---|---|
| `to-review/` | Gevonden prompts die je nog niet hebt gelezen of beoordeeld |
| `to-test/` | Prompts die je hebt gelezen en wilt uitproberen |

---

## ✍️ Hoe sla je iets op?

Maak een nieuw bestand aan in `to-review/` met een beschrijvende naam:

```
to-review/chatgpt-holy-grail-reasoning.md
to-review/x-thread-system-prompt-leak.md
```

Minimale inhoud — je hoeft alleen dit in te vullen:

```yaml
---
title: [titel of omschrijving]
source: [link of platform, bijv. x.com]
found: [datum, bijv. 2026-03-21]
status: unverified
---

[Plak hier de prompt letterlijk zoals je hem gevonden hebt]
```

Meer is niet nodig. De rest doe je tijdens je review.

---

## 🔄 Review-proces

Loop periodiek (wekelijks of maandelijks) je inbox door:

1. **Lees** de prompt — begrijp je wat hij doet?
2. **Test** hem met een model — werkt hij?
3. **Beoordeel** via `templates/evaluation-template.md`
4. **Verplaats** naar het juiste domein in `prompts/by-domain/`
5. **Vul** de volledige frontmatter in en verhoog de status naar `stable`

Wat niet werkt of geen meerwaarde heeft: gewoon verwijderen.

---

## 🏷️ Statusverloop

```
unverified  →  draft  →  tested  →  stable
```

| Status | Betekenis |
|---|---|
| `unverified` | Gevonden, nog niet gelezen of beoordeeld |
| `draft` | Gelezen, lijkt interessant, nog niet getest |
| `tested` | Getest, werkt, nog niet opgeschoond |
| `stable` | Volledig uitgewerkt, klaar voor hergebruik |

---

*De inbox is geen eindbestemming. Prompts die hier te lang blijven staan, worden verwijderd.*
