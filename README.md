# ZKEncrypt Documentationf

Official documentation site for ZKEncrypt Network - Built with VitePress.

## 🚀 Features

- **Comprehensive Guides**: Step-by-step tutorials for all skill levels
- **API Reference**: Complete SDK and contract documentation  
- **Interactive Examples**: Live code examples you can edit
- **Search**: Fast full-text search across all docs
- **Dark Mode**: Eye-friendly documentation reading

## 📖 Documentation Structure

```
docs/
├── guide/
│   ├── getting-started.md
│   ├── fhe-basics.md
│   ├── wallet-integration.md
│   └── deployment.md
├── sdk/
│   ├── installation.md
│   ├── api-reference.md
│   └── examples.md
├── contracts/
│   ├── fhe-operations.md
│   ├── confidential-erc20.md
│   └── deployment.md
├── cli/
│   ├── installation.md
│   └── commands.md
├── tutorials/
│   ├── first-dapp.md
│   ├── private-token.md
│   └── sealed-auction.md
└── api/
    ├── rest-api.md
    └── websocket.md
```

## 🛠️ Local Development

### Prerequisites

- Node.js >= 16
- npm or yarn

### Installation

```bash
npm install
```

### Development Server

```bash
npm run docs:dev
```

Visit `http://localhost:5173` to view the docs.

### Build

```bash
npm run docs:build
```

### Preview Build

```bash
npm run docs:preview
```

## 📝 Writing Documentation

### Create New Page

1. Add markdown file in `docs/` directory
2. Update `.vitepress/config.ts` sidebar
3. Add frontmatter:

```md
---
title: Your Page Title
description: Brief description
---

# Your Page Title

Content goes here...
```

### Code Examples

````md
```typescript
import { ZKEncryptSDK } from '@zkencrypt/sdk';

const sdk = new ZKEncryptSDK({
  network: 'mainnet-beta',
});
```
````

### Interactive Demos

Use custom Vue components for interactive examples:

```md
<FHEPlayground />
```

### Admonitions

```md
::: tip
This is a helpful tip
:::

::: warning
This is a warning
:::

::: danger
This is dangerous!
:::
```

## 🎨 Customization

### Theme Configuration

Edit `.vitepress/theme/index.ts`:

```typescript
import DefaultTheme from 'vitepress/theme';
import './custom.css';

export default {
  ...DefaultTheme,
  enhanceApp({ app }) {
    // Register custom components
  }
};
```

### Custom CSS

Add styles in `.vitepress/theme/custom.css`:

```css
:root {
  --vp-c-brand: #D2FD84;
  --vp-c-brand-dark: #00ff88;
}
```

## 📦 Deployment

### Deploy to Vercel

```bash
vercel --prod
```

### Deploy to Netlify

```bash
netlify deploy --prod
```

### Deploy to GitHub Pages

```bash
npm run docs:build
npm run docs:deploy
```

## 🔍 Search

Search is powered by Algolia DocSearch. Configuration:

```typescript
// .vitepress/config.ts
export default {
  themeConfig: {
    search: {
      provider: 'algolia',
      options: {
        appId: 'YOUR_APP_ID',
        apiKey: 'YOUR_API_KEY',
        indexName: 'zkencrypt'
      }
    }
  }
}
```

## 🤝 Contributing

Contributions welcome! Please:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

### Documentation Guidelines

- Use clear, concise language
- Include code examples
- Add images/diagrams when helpful
- Test all code examples
- Keep examples up to date

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

## 🔗 Links

- [Live Documentation](https://zkencrypt-ai.gitbook.io/zkencrypt-ai)
- [GitHub](https://github.com/ZKEncrypt-AI/zkencrypt-docs)
- [Website](https://zk-labs.network)

---

Built with ❤️ by the ZKEncrypt AI team
