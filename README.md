# pulsar

Organizations need a repeatable way to discover public-facing assets and check them as their infrastructure changes. pulsar helps security teams map domains and cloud resources, run scheduled checks, and review the results from one workspace.

## Features

- Discover subdomains and top-level domains for an organization.
- Find public cloud resources associated with a scan scope.
- Run basic vulnerability checks against discovered assets.
- Schedule scans and send notifications when checks complete.
- Visualize relationships between discovered resources and export scan data.
- Connect external APIs, OAuth providers, and custom scanner extensions.

## Installation

pulsar uses Node.js and npm for local development.

### Prerequisites

- Node.js 18 or newer
- npm 9 or newer

### Setup

```sh
git clone https://github.com/your-org/pulsar.git
cd pulsar
npm ci
npm run build
```

Start the application with:

```sh
npm start -- --host 0.0.0.0 --port 3000
```

Open `http://localhost:3000` in a browser. Review the project configuration before enabling external integrations or notifications.

## Usage

Run a scan for an authorized domain with the default policy:

```sh
npm run scan -- --domain example.com --policy default
```

Use only domains and infrastructure that you own or have explicit permission to assess. Scan results can then be reviewed in the web interface, exported, or used by scheduled checks.

## License

Apache-2.0. This project is based on [0x0FB0/pulsar](https://github.com/0x0FB0/pulsar), which was released under the Apache License 2.0. See [LICENSE](LICENSE) for the full license text and attribution details.
