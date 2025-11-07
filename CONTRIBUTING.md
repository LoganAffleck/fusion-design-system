# Contributing to Fusion Design System

Thank you for considering contributing to Fusion Design System! 🎉

## How to Contribute

### Reporting Bugs

1. Check if the bug has already been reported in [Issues](https://github.com/YOUR_USERNAME/fusion-design-system/issues)
2. If not, create a new issue using the Bug Report template
3. Provide as much detail as possible

### Suggesting Features

1. Check if the feature has already been suggested
2. Create a new issue using the Feature Request template
3. Explain the use case and benefits

### Pull Requests

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes**
   - Follow the existing code style
   - Add/update tests if applicable
   - Update documentation as needed

4. **Test your changes**
   ```bash
   npm run lint
   npm run type-check
   npm run build
   ```

5. **Commit your changes**
   ```bash
   git commit -m 'feat: add some feature'
   ```
   Use conventional commits:
   - `feat:` for new features
   - `fix:` for bug fixes
   - `docs:` for documentation
   - `style:` for formatting
   - `refactor:` for code refactoring
   - `test:` for tests
   - `chore:` for maintenance

6. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

7. **Open a Pull Request**
   - Provide a clear description
   - Link any related issues
   - Wait for review

## Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/fusion-design-system.git
cd fusion-design-system

# Install dependencies
npm install

# Build the package
npm run build

# Watch mode for development
npm run dev
```

## Code Style

- Use TypeScript for all code
- Follow the existing component patterns
- Use class-variance-authority for variants
- Ensure accessibility (ARIA attributes)
- Write clear comments for complex logic

## Component Guidelines

When adding a new component:

1. Create the component in `src/components/`
2. Export it from `src/index.ts`
3. Follow the existing pattern:
   - Use `React.forwardRef`
   - Support `className` prop
   - Use variants with `cva`
   - Include proper TypeScript types

## Questions?

Feel free to open a discussion or issue if you have questions!

Thank you for contributing! 🙏
