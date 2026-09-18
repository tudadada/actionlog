# actionlog

[![npm version](https://img.shields.io/npm/v/actionlog.svg)](https://www.npmjs.com/package/actionlog)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

**Tamper-Evident Autonomous Agent Action Audit & Governance Logging** MCP Server. Designed for AI agent compliance, recording irreversible audit trails and verifying tool execution integrity.

## Features

- **Cryptographic Audit Chain**: Every agent action, tool invocation, and API execution is hashed into a tamper-evident sequential log.
- **Agent Governance & Compliance**: Built for enterprise AI requirements (SOC2, EU AI Act traceability, agent liability auditing).
- **Model Context Protocol (MCP)**: Native integration for Claude Desktop, Cursor, and multi-agent orchestrators.

## Quick Start

### Direct Execution
```bash
npx actionlog
```

### Claude Desktop Integration

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "actionlog": {
      "command": "npx",
      "args": ["-y", "actionlog"]
    }
  }
}
```

## Tools Included

1. `record_agent_action`: Commits an agent action into the cryptographic hash chain.
2. `verify_log_integrity`: Validates historical log entries against checksum tampering.

## License

MIT © [tudadada](https://github.com/tudadada)
