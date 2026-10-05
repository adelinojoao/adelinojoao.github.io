# João Adelino — Personal Portfolio

Public website: https://adelinojoao.github.io/

Personal professional portfolio using Hugo Blox Academic CV, with a dark charcoal theme.

## Editing

- Profile and experience: `data/authors/me.yaml`
- Homepage sections: `content/pt/_index.md` and `content/en/_index.md`
- Projects: `content/pt/projects/<project>/index.md` and `content/en/projects/<project>/index.md`
- Navigation: `config/_default/menus.yaml`
- Colors and site metadata: `config/_default/params.yaml`
- Custom design: `assets/css/custom.css`
- Profile photograph: `assets/media/authors/me.jpg`

Project pages identify experimental work and projects still under development. No performance claims should be added without supporting results.

## Publishing

GitHub Actions builds the Hugo source and publishes the resulting `public/` directory through `.github/workflows/deploy.yml`. `hugoblox.yaml` selects `github-pages` as the deployment host. A separate hand-written root `index.html` is not used.

## Local preview

Install Hugo Extended 0.162.0, Go and Node.js 22. Install pnpm 10.14.0, then run:

```sh
pnpm install
hugo server
```

## Credits

Based on the Hugo Blox Academic CV starter. See `LICENSE.md` for the source template license.

## Languages

Brazilian Portuguese is the default at `/`; English is available at `/en/`. The PT-BR / EN switch links to the same page in the other language. Portuguese profile fields are in `data/pt/authors/me.yaml`; the English profile is in `data/authors/me.yaml`. Language-specific navigation and metadata are in `config/_default/languages.yaml`.
