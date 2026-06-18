# The Biased Judge

A field guide to LLM-as-a-Judge bias: why LLMs that grade other LLMs are quietly biased, the dozen documented ways it happens, and the practical moves that cancel each one out. Single self-contained page, light/dark theme, original writing and diagrams, with sources.

**Live site:** [https://aadityapanchal.github.io/llm-judge-bias/](https://aadityapanchal.github.io/llm-judge-bias/) *(after enabling GitHub Pages)*

## What is inside

- The premise: why we use LLM judges and where the trust breaks
- A pipeline diagram showing the three places a verdict bends
- The Charges: ~13 biases grouped into Presentation, Ego and lineage, Persuasion, and Reasoning blind spots
- The Defense: nine mitigation moves, each mapped to the biases it cancels
- A calibration-loop diagram and a one-screen cheat sheet
- 11 sourced references (papers and surveys)

## Enable GitHub Pages

1. Push `index.html` to the `main` branch
2. Repo **Settings > Pages**
3. Source: **Deploy from a branch**
4. Branch: **main**, folder: **/ (root)**
5. Save. Live in about 1 to 2 minutes at the URL above

## Local preview

Open `index.html` in a browser, or:

```bash
python3 -m http.server 8080
# visit http://localhost:8080
```

## Push changes (personal account, no saved credentials)

```bash
cd /Users/aditya.panchal/Desktop/temp
git add index.html README.md
git commit -m "Redesign: field-guide layout, expanded biases, light/dark theme"
git -c credential.helper= push origin main
```

Use your personal PAT when prompted for the password.

## Notes

All writing and diagrams are original. Every numeric claim traces to a paper in the Sources section, not to a third-party graphic.
