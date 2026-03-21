# 🤝 Contributing to Prompt OS

Bedankt dat je wilt bijdragen aan Prompt OS. Dit document beschrijft hoe je prompts, frameworks, templates en evaluaties toevoegt op een manier die consistent blijft met de rest van het systeem.

---

## 📐 Uitgangspunten

- **Kwaliteit boven kwantiteit** — één goed uitgewerkte prompt is meer waard dan tien halfbakken varianten
- **Structuur is niet optioneel** — gebruik altijd de juiste template en naamgevingsconventie
- **Documenteer je keuzes** — een prompt zonder context is een prompt die niemand hergebruikt
- **Test voor je commit** — voeg minimaal één input/output-voorbeeld toe

---

## 🗂️ Wat kun je bijdragen?

| Type | Map | Template |
|---|---|---|
| Losse prompt | `prompts/by-domain/<domein>/` | `templates/prompt-template.md` |
| Systeemprompt | `prompts/systems/<systeem>/` | `templates/system-prompt-template.md` |
| Framework | `frameworks/` | — |
| Evaluatie | `evaluations/` | `templates/evaluation-template.md` |
| Workflow | `prompts/systems/` | `templates/workflow-template.md` |
| Voorbeeld | `examples/` | — |

---

## ✍️ Naamgevingsconventies

Gebruik altijd de volgende structuur voor bestandsnamen:

```
<domein>-<type>-<onderwerp>.md
```

**Voorbeelden:**

```
business-strategy-market-entry.md
finance-analysis-investment-thesis.md
productivity-planning-weekly-review.md
```

Regels:
- Alles **lowercase**
- Woorden gescheiden door **koppeltekens** (`-`), geen underscores
- Geen spaties, geen speciale tekens
- Begin altijd met het domein, dan het type, dan het onderwerp

Zie [`docs/naming-conventions.md`](docs/naming-conventions.md) voor het volledige overzicht.

---

## 🏷️ Tagging

Elke prompt krijgt tags bovenaan het bestand in de frontmatter:

```yaml
---
title: Market Entry Strategy
domain: business
type: strategy
tags: [market-entry, competitive-analysis, go-to-market]
model: claude-sonnet
version: 1.0.0
status: stable
---
```

Gebruik bestaande tags waar mogelijk. Nieuwe tags voeg je toe aan [`docs/tagging-system.md`](docs/tagging-system.md).

---

## 📋 Stappenplan voor een nieuwe prompt

**1. Kies de juiste template**

```bash
cp templates/prompt-template.md prompts/by-domain/<domein>/<naam>.md
```

**2. Vul de frontmatter in**

Titel, domein, type, tags, model en versie — alles ingevuld vóór je verder schrijft.

**3. Schrijf de prompt**

Gebruik een van de frameworks uit `frameworks/` als basis. Documenteer:
- Het doel van de prompt
- De aannames over de gebruiker of context
- Variabelen die vervangen moeten worden (gebruik `{{dubbele accolades}}`)

**4. Voeg een voorbeeld toe**

Minimaal één concreet input/output-paar in `examples/input-output-pairs/`.

**5. Evalueer**

Gebruik `templates/evaluation-template.md` om de kwaliteit te beoordelen. Voeg het toe aan `evaluations/scorecards/`.

**6. Commit met een duidelijk bericht**

```bash
git add .
git commit -m "feat(prompts): add business-strategy-market-entry v1.0.0"
```

---

## 🔢 Versiebeheer

Versies volgen [Semantic Versioning](https://semver.org/):

| Versie | Wanneer |
|---|---|
| `1.0.0` | Eerste stabiele versie |
| `1.1.0` | Nieuwe functionaliteit of uitbreiding |
| `1.0.1` | Kleine correctie of verduidelijking |
| `2.0.0` | Fundamentele herschrijving |

Zie [`docs/versioning-rules.md`](docs/versioning-rules.md) voor details.

---

## 🌿 Branchstrategie

| Branch | Gebruik |
|---|---|
| `main` | Stabiele, geteste prompts |
| `draft/<naam>` | Prompts in ontwikkeling |
| `fix/<naam>` | Correcties op bestaande prompts |
| `feat/<naam>` | Nieuwe domeinen of systemen |

Maak altijd een pull request aan vanuit een feature branch — commit nooit direct op `main`.

---

## ✅ Review checklist

Voordat een bijdrage wordt samengevoegd, controleer je:

- [ ] Bestandsnaam volgt de naamgevingsconventie
- [ ] Frontmatter volledig ingevuld
- [ ] Prompt getest met minimaal één model
- [ ] Input/output-voorbeeld toegevoegd
- [ ] Evaluatie ingevuld
- [ ] Versienummer correct
- [ ] CHANGELOG.md bijgewerkt

---

## 📬 Vragen?

Open een [issue](../../issues) of start een discussie. Bijdragen zijn altijd welkom — groot of klein.

---

*Samen bouwen we een promptsysteem dat echt werkt.*
