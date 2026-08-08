# Git Branch Naming

```bash
# Optimal Branch Exmplar: 

> git branch -v
    main
    * type/scope/description
```

Types
- `feat` —  a new feature or capability
- `fix` —  a bug fix (not bugfix — just fix)
- `refactor` —  code change that neither fixes a bug nor adds a feature (restructuring, renaming, decoupling)
- `chore` —  maintenance work with no production code change (deps, config, tooling)
- `docs` —  documentation only
- `style` —  formatting/whitespace only, no logic change 
    - (careful: this is a specific narrow meaning — Biome/lint fixes that touch actual logic branches would be fix or chore, not style)
- `test` —  adding or fixing tests, no production code change
- `ci` —  changes to CI configuration/scripts (what you've been using for the workflow files)
- `build` —  changes to the build system or external dependencies (webpack, bun config, Docker as a build tool)
- `perf` —  a code change that improves performance
- `revert` —  reverts a previous commit

Scopes:
- `type/frontend`
- `type/api`
- `type/build`
---
- `fix/ci`
- `chore/install-deps`
- `style/frontend`
- `test/api`

Descriptions:
These shouldn't be crazy long but descriptive enough
- `feat/api/cors`
- `test/api/units`
- `fix/api/buffer-overflow`
