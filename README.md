# Codie

Code on the go controlling claude code from your mobile device.

Free. Open source. Code anywhere.

## Installation

```bash
npm install -g Codie-coder
```

## Usage

```bash
Codie
```

This will:
1. Start a Claude Code session
2. Display a QR code to connect from your mobile device
3. Allow real-time session sharing between Claude Code and your mobile app

## Commands

- `Codie auth` – Manage authentication
- `Codie codex` – Start Codex mode
- `Codie connect` – Store AI vendor API keys in Codie cloud
- `Codie notify` – Send a push notification to your devices
- `Codie daemon` – Manage background service
- `Codie doctor` – System diagnostics & troubleshooting

## Options

- `-h, --help` - Show help
- `-v, --version` - Show version
- `-m, --model <model>` - Claude model to use (default: sonnet)
- `-p, --permission-mode <mode>` - Permission mode: auto, default, or plan
- `--claude-env KEY=VALUE` - Set environment variable for Claude Code
- `--claude-arg ARG` - Pass additional argument to Claude CLI

## Environment Variables

- `Codie_SERVER_URL` - Custom server URL (default: https://api.cluster-fluster.com)
- `Codie_WEBAPP_URL` - Custom web app URL (default: https://app.Codie.engineering)
- `Codie_HOME_DIR` - Custom home directory for Codie data (default: ~/.Codie)
- `Codie_DISABLE_CAFFEINATE` - Disable macOS sleep prevention (set to `true`, `1`, or `yes`)
- `Codie_EXPERIMENTAL` - Enable experimental features (set to `true`, `1`, or `yes`)

## Requirements

- Node.js >= 20.0.0
  - Required by `eventsource-parser@3.0.5`, which is required by
  `@modelcontextprotocol/sdk`, which we used to implement permission forwarding
  to mobile app
- Claude CLI installed & logged in (`claude` command available in PATH)

## License

MIT
