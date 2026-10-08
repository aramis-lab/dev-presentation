# Template for developer presentations

To build HTML slides from Markdown files, like [this one](https://www.aramislab.fr/dev-presentation/).

This repo was generated with the tool [Slidev](https://sli.dev/).

## Installation

### Install Node.js

Install `Node.js`:
```bash
brew install node@24
```

Check `Node.js` version:
```bash
node -v # must return v24.21.0
```

Check `npm` version:
```bash
npm -v # must return 11.19.0
```

### Install the dependencies

```bash
npm install
```

## To start the slide show

Run:
```bash
npm run dev
```

You can see that the presentation content is defined in the markdown file [slides.md](./slides.md). Besides, it can also integrate the content of auxiliary markdown files, like [pages/imported-slides.md](./pages/imported-slides.md), which is useful if you want to build a presentation from multiple files.

## To modify the presentation

Edit the [slides.md](./slides.md) to see the changes.

Learn more about Slidev at the [documentation](https://sli.dev/).

## To deploy your presentation online

`npm run dev` enables to open your presentation locally. If you want to deploy the presentation online, for example to share it, do the following steps:

1. On GitHub, go to `Settings` > `General` > `Danger Zone` > `Change repository visibility`, and make sure that the repository is public.
2. Then `Settings` > `Pages` > `Build and deployment`, and select `GitHub Actions`.
3. Commit something on your `main` branch (for example an empty commit with `git commit --allow-empty -m "trigger documentation deployment"`) and push it on GitHub.
4. On your repository main page, check that the deployment is successful in the section `Deployments` (you may have to refresh).
5. Your presentation should be available at `https://www.aramislab.fr/<repo-name>/` (or `http://www.aramislab.fr/<repo-name>/`).

The presentation will be rebuilt and deployed automatically every time you push on the `main` branch!