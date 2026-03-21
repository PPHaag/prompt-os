# 🧠 Prompt OS

> Een gestructureerd systeem voor het bouwen, opslaan, evalueren en hergebruiken van AI-prompts.

Prompt OS is een persoonlijke kennisbank en werkinfrastructuur voor iedereen die serieus werkt met AI-taalmodellen. In plaats van prompts los op te slaan in notities of chats, biedt dit systeem een consistente mappenstructuur, naamgevingsconventies, templates en evaluatiekaders — zodat je prompts schaalbaar, vindbaar en herbruikbaar worden.

---

## 🚀 Waarom Prompt OS?

De meeste mensen verliezen hun beste prompts. Ze staan verspreid over chats, notities en documenten — zonder context, zonder versie, zonder structuur.

Prompt OS lost dat op met:

- **Consistente structuur** — elke prompt op dezelfde plek, in hetzelfde formaat
- **Domeingericht opslaan** — business, finance, productiviteit, en meer
- **Herbruikbare frameworks** — denkkaders die je steeds opnieuw kunt inzetten
- **Evaluatie ingebouwd** — benchmarks, scorecards en testcases naast je prompts
- **Klaar voor samenwerking** — GitHub-native, met bijdragerichtlijnen en versiebeheer

---

## 📁 Structuur

```
.
├── prompts/              # Alle prompts, per domein en systeem
│   ├── by-domain/        # Domeinspecifieke prompts
│   └── systems/          # Systeem-level agents en workflows
├── frameworks/           # Herbruikbare promptkaders
├── templates/            # Startbestanden voor nieuwe prompts
├── evaluations/          # Benchmarks, scorecards en testcases
├── examples/             # Ingevulde voorbeelden en use cases
├── docs/                 # Conventies, taxonomie en roadmap
├── ARCHITECTURE.md       # Hoe het systeem is opgebouwd
├── CONTRIBUTING.md       # Hoe bij te dragen
└── CHANGELOG.md          # Wat er veranderd is
```

---

## 🗂️ Promptdomeinen

Prompts zijn georganiseerd op domein onder `prompts/by-domain/`:

| Domein | Voorbeeldprompt |
|---|---|
| 🏢 Business | `business-strategy-market-entry.md` |
| 💰 Finance | `finance-analysis-investment-thesis.md` |
| ✅ Productiviteit | `productivity-planning-weekly-review.md` |

Nieuw domein toevoegen? Maak een map aan onder `by-domain/` en volg de naamgevingsconventie in [`docs/naming-conventions.md`](docs/naming-conventions.md).

---

## 🧠 Frameworks

Onder `frameworks/` staan herbruikbare denk- en promptkaders:

| Framework | Gebruik |
|---|---|
| `role-task-format.md` | Basiskader: rol → taak → formaat |
| `chain-of-thought-safe.md` | Stap-voor-stap redeneren |
| `critique-and-rewrite.md` | Output verbeteren via zelfkritiek |
| `decision-framework.md` | Gestructureerde besluitvorming |
| `prompt-optimization-loop.md` | Iteratief verbeteren van prompts |

---

## ⚙️ Systemen

Onder `prompts/systems/` staan kant-en-klare AI-systemen:

| Systeem | Functie |
|---|---|
| `advisor-engine/` | Strategisch advies genereren |
| `agent-workflows/` | Meertraps taakuitvoering |
| `content-engine/` | Content schrijven en bewerken |
| `research-engine/` | Onderzoek en synthese |
| `strategy-engine/` | Strategisch redeneren |

---

## 📋 Templates

Start een nieuwe prompt altijd vanuit een template in `templates/`:

- **`prompt-template.md`** — voor losse prompts
- **`system-prompt-template.md`** — voor systeem-level instructies
- **`evaluation-template.md`** — voor het beoordelen van output
- **`workflow-template.md`** — voor meerstaps processen

---

## 🧪 Evaluatie

Elke prompt kan geëvalueerd worden via de structuur in `evaluations/`:

- `benchmarks/` — prestaties over tijd bijhouden
- `model-comparisons/` — verschillende modellen vergelijken
- `scorecards/` — vaste beoordelingscriteria
- `test-cases/` — scenario's om prompts te testen

---

## 📖 Documentatie

| Doc | Inhoud |
|---|---|
| [`docs/naming-conventions.md`](docs/naming-conventions.md) | Hoe bestanden te benoemen |
| [`docs/taxonomy.md`](docs/taxonomy.md) | Categorisatiesysteem |
| [`docs/tagging-system.md`](docs/tagging-system.md) | Tags per prompt |
| [`docs/versioning-rules.md`](docs/versioning-rules.md) | Versiebeheer |
| [`docs/roadmap.md`](docs/roadmap.md) | Wat er nog komt |

---

## 🛠️ Installatie

```bash
git clone https://github.com/jouwgebruikersnaam/prompt-os.git
cd prompt-os
bash setup-prompt-os.sh
```

---

## 🤝 Bijdragen

Wil je een prompt, framework of template toevoegen? Lees [`CONTRIBUTING.md`](CONTRIBUTING.md) voor de richtlijnen.

---

*Gebouwd voor iedereen die AI serieus neemt.*
