[![npm version](https://badge.fury.io/js/agentic.md.svg)](https://badge.fury.io/js/agentic.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# agentic.md

Build, Test, Deploy, & Iterate on AI Agents using Markdown & MDX

## Overview

`agentic.md` is a powerful npm package that enables you to create, test, and deploy AI agents using the simplicity of Markdown and the extensibility of MDX. By combining the ease of markdown with the power of MDX components, you can rapidly prototype and iterate on AI agents.

## Features

- 🚀 **Quick Start**: Build AI agents using familiar Markdown syntax
- 🧪 **Testing Framework**: Built-in tools for testing agent behaviors
- 📦 **Easy Deployment**: Streamlined deployment process
- 🔄 **Rapid Iteration**: Fast feedback loop for agent development
- 📝 **MDX Integration**: Leverage React components in your agent definitions

## Installation

```bash
npm install agentic.md
# or
yarn add agentic.md
# or
pnpm add agentic.md
```

## Usage

```jsx
import { Agent } from 'agentic.md';

const MyAgent = () => (
  <Agent
    source='# My AI Agent

    ## System Prompt
    You are a helpful assistant.

    ## Actions
    - search: Search the web
    - respond: Respond to user
    '
  />
);
```

## Documentation

### Creating an Agent

Create your agent using standard Markdown with MDX components:

```md
# Customer Service Agent

## System Prompt
You are a friendly customer service representative.

## Actions
- lookup_order: Look up order status
- respond: Send message to customer
```

### Testing

Test your agents using the built-in testing utilities:

```jsx
import { test } from 'agentic.md/testing';

test('agent responds correctly', async () => {
  const response = await agent.respond('What is my order status?');
  expect(response).toContain('order status');
});
```

### Deployment

Deploy your agents easily:

```jsx
import { deploy } from 'agentic.md/deploy';

await deploy(agent, {
  environment: 'production',
  version: '1.0.0'
});
```

## Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

## License

MIT License - see the [LICENSE](LICENSE) file for details.

## Dependencies

- React ^18.0.0
- MDX ^2.0.0
- OpenAI API (for AI capabilities)
