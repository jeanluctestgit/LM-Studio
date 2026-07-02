# LM Studio 1.0 — Fondations

LM Studio devient un projet unique et pérenne.

Objectif :
décrire une leçon de guitare une seule fois, puis générer automatiquement plusieurs formats :

- SVG
- HTML interactif
- EPUB
- PDF
- ODT
- JSON

## Structure

```text
LM_Studio_1_0_foundations/
├── apps/
│   ├── cli/
│   ├── studio/
│   └── player/
├── packages/
│   ├── lm_core/
│   ├── lm_dsl/
│   ├── lm_timeline/
│   ├── lm_assets/
│   ├── lm_widgets/
│   ├── lm_render_svg/
│   ├── lm_render_html/
│   ├── lm_render_epub/
│   ├── lm_render_pdf/
│   ├── lm_render_odt/
│   └── lm_runtime/
├── widgets/
├── assets/
├── examples/
├── tests/
├── docs/
├── templates/
└── output/
```

## Premier test

```powershell
python apps/cli/lm.py inspect examples/Volume0/LM-C05-B_Tresillo.lm
python apps/cli/lm.py build examples/Volume0/LM-C05-B_Tresillo.lm --html --svg
```

Les sorties apparaissent dans :

```text
output/html/
output/svg/
```
