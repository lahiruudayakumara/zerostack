# ZeroStack

ZeroStack is a modern, extensible serverless framework CLI and core library designed to help developers easily scaffold, build, and deploy serverless applications.

---

## Repository Structure

```
zerostack/
├── packages/
│   ├── cli/                      # CLI tool (npm package)
│   ├── core/                     # Core shared utilities and AWS abstractions
├── templates/                    # Default serverless project templates 
├── docs/                         # Documentation site powered by Next.js
├── scripts/                      # Build, release, deploy scripts
├── .gitignore
├── package.json                  # Root workspace config (pnpm/yarn workspaces)
├── pnpm-workspace.yaml
└── README.md
```

---

## Features

- **CLI tool** (`zerostack`): Scaffold projects (`init`), deploy services (`deploy`), and more.
- **Core library**: Shared utilities for AWS deployments and infrastructure.
- **Project templates**: Quickly scaffold starter projects like hello-world and API services.
- **Documentation site**: Built with Next.js, live at `/docs`.
- **Monorepo**: Using pnpm workspaces for clean dependency management and development.

---

## Getting Started

### Prerequisites

- Node.js >= 18
- pnpm (recommended) or npm/yarn

### Installation

First, fork this repository on GitHub to your own account.

Then clone your fork and install dependencies:

```bash
git clone https://github.com/your-username/zerostack.git
cd zerostack
pnpm install
```

### Using the CLI

To link the CLI tool globally for local development:

```bash
cd packages/cli
npm link
```

Now you can use the CLI globally:

```bash
zerostack init          # Scaffold a new project from templates
zerostack deploy        # Deploy your serverless project (stub implementation)
```

---

## Documentation

The documentation site is built with Next.js and lives in the `docs/` folder.

To run the docs locally:

```bash
cd docs
pnpm dev
```

Open your browser at [http://localhost:3000](http://localhost:3000) to view docs.

---

## Scripts

Run these commands from the root directory using pnpm:

| Command       | Description                               |
|---------------|-------------------------------------------|
| `pnpm build`  | Build all packages                        |
| `pnpm test`   | Run tests for all packages                |
| `pnpm lint`   | Run linters on all packages               |
| `pnpm docs:dev` | Run the docs site locally               |
| `pnpm docs:build` | Build static docs site                  |
| `pnpm docs:start` | Serve built docs site locally          |

---

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check issues or submit pull requests.

---

## License

This project is licensed under the Apache License 2.0. See the [LICENSE](./LICENSE) file for details.

---