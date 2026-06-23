# projects-template-registry

`projects-template-registry` is the manifest registry for `stripe projects build`.

Each YAML file describes a build template that the CLI can discover, filter, and materialize. The registry does not contain the starter app code itself. A manifest can point to any compatible public GitHub repository and pinned commit.

For an example of a public template repo, see Stripe's [`projects-templates`](https://github.com/stripe/projects-templates) repository.

## What the registry controls

- Search and browse metadata shown in the CLI
- Guided-flow placement by category and framework
- Variant grouping and ordering
- The pinned git commit users receive
- Declared Stripe Projects services and post-setup commands

## Repository layout

- `guided.yaml`: guided-flow category labels and descriptions
- `<category>/<variant>.yaml`: template manifests consumed by the CLI
- `example/example.yaml`: commented reference manifest for contributors

## Contributing

Add or update manifests here when you want a template from any public repo to appear in `stripe projects build`. See [CONTRIBUTING.md](CONTRIBUTING.md) for the expected manifest workflow.

## Security

See [SECURITY.md](SECURITY.md) for vulnerability reporting instructions.
