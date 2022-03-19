## Monorepo Seed

Built with Rush to provide a baseline set of tooling so you can skip right to the good stuff.

### Features

#### Dev 🤯

All projects can be built as changes are made via watch mode given they define a `rush:build:watch` script.  
This enables a workflow where the dependency tree can be worked on without explicitly building each project.

```
Project B depends on Project A
rush rush:build:watch
```

When in watch mode, Project A can make breaking changes that are immediately reflected in Project B.  
If Project A has in progress changes that keep it from building, Project B will be unaffected until Project A builds.

#### Testing 🧪

#### Linting 🔎

Linting can be invoked manually on staged files by running `rush lint-staged`.

`lint-staged` pre commit hook that applies

- `eslint` to JavaScript and TypeScript
- `stylelint` to (S)CSS
- `prettier` to JavaScript, TypeScript, (S)CSS, and Markdown

#### Publishing 🚀
