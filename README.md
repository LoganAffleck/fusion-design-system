# Fusion Design System

A modern, accessible design system built with React, TypeScript, and Tailwind CSS. Inspired by [Shadcn/ui](https://ui.shadcn.com/) and optimized for Builder.io integration.

[![TypeScript](https://img.shields.io/badge/TypeScript-5.9-blue)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-18.3-blue)](https://react.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4-blue)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## ✨ Features

- 🎨 **Modern Component Library** - Production-ready React components
- 🔧 **Fully Typed** - Built with TypeScript for complete type safety
- 🎭 **Variant System** - Using class-variance-authority for flexible styling
- 🌓 **Dark Mode Ready** - CSS variables for easy theming
- 📦 **Tree-shakeable** - ESM and CJS builds with tsup
- ♿ **Accessible** - ARIA-compliant components with Radix UI primitives
- 🔌 **Builder.io Ready** - Designed for visual editing integration

## 📦 Installation

### As NPM Package (Recommended for Publishing)
```bash
npm install @fusion/design-system
# or
yarn add @fusion/design-system
# or
pnpm add @fusion/design-system
```

### As Local Workspace Package
For monorepo or local development:

```json
{
  "dependencies": {
    "@fusion/design-system": "file:../design-system"
  }
}
```

## 🚀 Quick Start

Import components directly:

```tsx
import { Button, Card, CardHeader, CardTitle, CardContent } from "@fusion/design-system"

export function MyComponent() {
  return (
    <Card>
      <CardHeader>
        <CardTitle>Hello World</CardTitle>
      </CardHeader>
      <CardContent>
        <Button>Click me</Button>
      </CardContent>
    </Card>
  )
}
```

## 🚀 Quick Start

Import components directly:

```tsx
import { Button, Card, CardHeader, CardTitle, CardContent } from "@fusion/design-system"

export function MyComponent() {
  return (
    <Card>
      <CardHeader>
        <CardTitle>Hello World</CardTitle>
      </CardHeader>
      <CardContent>
        <Button variant="default">Click me</Button>
      </CardContent>
    </Card>
  )
}
```

## 🧩 Available Components

### Button
```tsx
<Button variant="default">Default</Button>
<Button variant="destructive">Destructive</Button>
<Button variant="outline">Outline</Button>
<Button variant="secondary">Secondary</Button>
<Button variant="ghost">Ghost</Button>
<Button variant="link">Link</Button>

// Composition with asChild
<Button asChild>
  <Link href="/dashboard">Dashboard</Link>
</Button>
```

### Card
```tsx
<Card>
  <CardHeader>
    <CardTitle>Title</CardTitle>
    <CardDescription>Description</CardDescription>
  </CardHeader>
  <CardContent>Content</CardContent>
  <CardFooter>Footer</CardFooter>
</Card>
```

### Input, Textarea, Badge
```tsx
<Input type="email" placeholder="Email..." />
<Textarea placeholder="Message..." />
<Badge variant="default">New</Badge>
```

## 🎨 Theming

Uses CSS variables for customization. See your app's `globals.css` for theme configuration.

## 🔧 Development Scripts

Build the package:

```bash
npm run build
```

Watch mode for development:

```bash
npm run dev
```

Lint and type-check:

```bash
npm run lint
npm run type-check
```

## 🏗️ Built With

- **[React 18](https://react.dev/)** - UI library
- **[TypeScript](https://www.typescriptlang.org/)** - Type safety
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS
- **[class-variance-authority](https://cva.style/)** - Variant management
- **[Radix UI](https://www.radix-ui.com/)** - Accessible primitives (Slot)
- **[tsup](https://tsup.egoist.dev/)** - TypeScript bundler

## 📁 Project Structure

```
design-system/
├── src/
│   ├── components/
│   │   ├── button.tsx
│   │   ├── card.tsx
│   │   ├── input.tsx
│   │   ├── textarea.tsx
│   │   └── badge.tsx
│   ├── lib/
│   │   └── utils.ts
│   └── index.ts
├── dist/              # Build output (CJS, ESM, types)
├── package.json
├── tsconfig.json
└── README.md
```

## 📄 License

MIT License - see [LICENSE](LICENSE) for details

## 🤝 Contributing

Contributions welcome! Please open an issue or submit a PR.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 🔗 Related Projects

- **[Fusion App](https://github.com/LoganAffleck/fusion-app)** - Next.js app using this design system
- **[Shadcn/ui](https://ui.shadcn.com/)** - Design inspiration

---

Made with ❤️ for modern web development
