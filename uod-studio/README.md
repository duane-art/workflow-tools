# UoD Studio

A suite of prompt instruments for the **Universes of Devotion** AI video pipeline. Each tool is a self-contained HTML page — no build step, no backend — that assembles a prompt you paste where it's needed. Together they carry a concept from idea to finished shots.

**Live:** https://duane-art.github.io/workflow-tools/uod-studio/

## The pipeline

The studio moves a project through three stages, and the launchpad ties them together:

1. **Orchestrate** — shape the concept and let The Planner and The Prompter build the plan, character sheets, and storyboards.
2. **Vary** — explore the look: generate a graded set of image-prompt variations on a key frame or subject.
3. **Make shots** — turn a chosen image into ready-to-run prompts for the image and video generators.

Each tool only *assembles* a prompt or payload; the generation happens in ChatGPT, Grok, Gemini, or your video generator of choice.

## The tools

| File | What it does |
|------|--------------|
| `index.html` | **Studio launchpad** — the suite home. Links every instrument as a numbered pipeline. |
| `UoD_Studio.html` | The launchpad's original file, kept as a stable target for the tools' back-links. |
| `UoD_Comet_Orchestrator.html` | **Orchestrator** — shapes a concept and stamps it into the Comet automation payload that drives **The Planner** and **The Prompter** through plan → character sheets → storyboards. Ingests a Final Draft `.fdx` script *or* a fillable **Creator Doc** intake form (PDF), whose structured per-character spec sheets flow straight into photoreal identity sheets. Built-in Writer, Creator, and Run-parameters readmes. |
| `UoD_Variations.html` | **Variations** — a graded intensity ladder of image-prompt variations (Subtle → Radical) with selectable line styles, for visual development on a single subject or frame. |
| `UoD_Shot_Maker.html` | **Shot Maker** — turns a reference image into ready-to-run shot / render prompts: the bridge from a look to finished frames. |

## Running them

Every page is fully self-contained — open any `.html` in a browser and it works offline (the Orchestrator's fillable PDF is embedded right in the page). Or use the hosted versions:

- Studio home — `https://duane-art.github.io/workflow-tools/uod-studio/`
- Orchestrator — `…/uod-studio/UoD_Comet_Orchestrator.html`
- Variations — `…/uod-studio/UoD_Variations.html`
- Shot Maker — `…/uod-studio/UoD_Shot_Maker.html`

## Licensed tools

The Orchestrator's payloads call **The Planner** and **The Prompter** by name (`@planner`, `@prompter`). These are proprietary custom GPTs built by **UoD LABS** and are **not** bundled with these pages — sharing the HTML does not grant access. Each user must have The Planner and The Prompter in their own ChatGPT GPT list. To request a license, contact UoD LABS at **hello@uodstudios.ai**.

## License

MIT. The HTML is openly forkable; the tools only assemble prompts and are inert without the licensed GPTs above.

---

*UoD Studio — instruments by Duane Loose.*
