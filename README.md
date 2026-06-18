# blogs

A small collection of self-contained writing on language models, agents, and evaluation. Each post is its own folder with a single `index.html` (light/dark theme, original writing and diagrams, sources included). A landing page at the root links to every post.

**Live site:** [https://aadityapanchal.github.io/blogs/](https://aadityapanchal.github.io/blogs/) *(after enabling GitHub Pages)*

## Structure

```
blogs/
|-- index.html              landing page that links to each post
|-- README.md
|-- llm-judge-bias/
|   |-- index.html          post -> /blogs/llm-judge-bias/
|-- <future-post>/
|   |-- index.html          post -> /blogs/<future-post>/
```

GitHub Pages serves from the repo root, so every folder with an `index.html` is published automatically.

## Posts

- **Judging the Agent: LLM-as-a-Judge Bias in Agentic Systems** -> [`llm-judge-bias/`](llm-judge-bias/)
  Why LLM judges that grade agentic systems are biased, where the agent setting makes it worse, and the moves that fix it.

## Add a new post

1. Create a folder, for example `my-topic/`
2. Add `my-topic/index.html`
3. Add a card linking to `my-topic/` in the root `index.html`
4. Commit and push. It goes live at `/blogs/my-topic/`

## Enable GitHub Pages

1. Push to the `main` branch
2. Repo **Settings > Pages**
3. Source: **Deploy from a branch**
4. Branch: **main**, folder: **/ (root)**
5. Save. Live in about 1 to 2 minutes

## Local preview

```bash
python3 -m http.server 8080
# landing page:  http://localhost:8080/
# the post:      http://localhost:8080/llm-judge-bias/
```

## Push changes (personal account, no saved credentials)

If you renamed the repo from `llm-judge-bias` to `blogs`, point your local remote at the new name first:

```bash
cd /Users/aditya.panchal/Desktop/temp
git remote set-url origin https://github.com/aadityapanchal/blogs.git
```

Then commit and push:

```bash
git add .
git commit -m "Restructure into multi-post blogs repo; make post agent-specific"
git -c credential.helper= push origin main
```

Use your personal PAT when prompted for the password.

## Notes

All writing and diagrams are original. Every claim traces to a paper in each post's Sources section, not to a third-party graphic.
