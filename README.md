# UoD Studio

A suite of prompt instruments for the **Universes of Devotion** AI video pipeline. Each tool is a self-contained HTML page — no build step, no backend — that assembles a prompt you paste where it's needed. Together they carry a concept from idea to finished shots.

## The pipeline

```
concept → prompts & storyboards → variations → reference → shots
```

| # | Tool | File | What it does |
|---|------|------|--------------|
| 00 | **Studio** | `index.html` | The home page. Links the suite together. |
| 01 | **Orchestrator** | `UoD_Comet_Orchestrator.html` | Shapes a concept and builds the Comet automation payload that drives ChatGPT (and optionally renders in Grok or Gemini) through prompts, character sheets, and storyboards. |
| 02 | **Variations** | `UoD_Variations.html` | Spins variations off a storyboard frame, character sheet, or any image. The keepers become reference for the next step. |
| 03 | **Shot maker** | `UoD_Shot_Maker.html` | Builds still and motion prompts off a chosen reference — shot type, camera move, and sound. |

## Running it

Open `index.html` and follow the cards top to bottom. Each tool builds a prompt and gives you a copy button; you paste that prompt into the relevant app (Comet's assistant for the Orchestrator; ChatGPT / Nano Banana / Veo for the others) with your reference images uploaded.

**Platforms (Orchestrator):** planning always runs in ChatGPT via the Planner and Prompter GPTs. The platform selector chooses where images render — ChatGPT (same chat, zips the assets), Grok, or Gemini (new tab, downloads images). For Grok and Gemini, be signed into both ChatGPT and the render platform.

## ⚠ Licensed tools — access required

**The Planner** and **The Prompter** are proprietary custom GPTs built by UoD LABS. The Orchestrator's payloads call them by name (`@planner`, `@prompter`) and cannot function without them. They are licensed for use within Universes of Devotion and are **not** included with these tools — each user must have them in their own ChatGPT GPT list.

To request a license, contact **UoD LABS — hello@uodstudios.ai**.

## Deploy / update on GitHub

This suite lives in the `uod-studio/` folder of the `duane-art/workflow-tools` repo, served by GitHub Pages.

To deploy or update:

1. Open the repo and go into the `uod-studio/` folder (or create it on first upload).
2. Click **Add file → Upload files** and drag in all five files below. Keep the filenames exactly — the cross-links are case-sensitive.
3. Commit to the `main` branch.
4. Pages is already enabled, so the site republishes within ~1 minute.

*First-time Pages setup only:* repo **Settings → Pages → Source: Deploy from a branch → `main` / root → Save.**

### Live links

- **Suite home** — https://duane-art.github.io/workflow-tools/uod-studio/
- Orchestrator — https://duane-art.github.io/workflow-tools/uod-studio/UoD_Comet_Orchestrator.html
- Variations — https://duane-art.github.io/workflow-tools/uod-studio/UoD_Variations.html
- Shot maker — https://duane-art.github.io/workflow-tools/uod-studio/UoD_Shot_Maker.html

## Notes

- These tools build prompts; they do not generate images or video themselves.
- All data lives in the page during a session. Use the Orchestrator's **Export library** to save your concepts to a JSON file you can commit alongside the tools.

---

*A UoD instrument suite — Duane Loose · UoD LABS*
