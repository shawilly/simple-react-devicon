# 📦 Publish `react-simple-devicons` to npm

This guide provides instructions to publish the `react-simple-devicons` package to npm.

## Prerequisites

Ensure you have:

1. An npm account. You can [create one here](https://www.npmjs.com/signup) if needed.
2. Logged in to npm in your terminal. Use:

   ```bash
   pnpm login
   ```

## Build and Publish `react-simple-devicons`

1. **Build the package**

   Use `tsup` to bundle `react-simple-devicons` for production:

   ```bash
   pnpm build
   ```

2. **Versioning and Releasing**

   Run `release-it` to create a new semantic version tag, push it to GitHub, and trigger a GitHub Action to build and publish your package if configured:

   ```bash
   pnpm release
   ```

3. **Manual Publish to npm**

   If you prefer to publish directly to npm without using GitHub Actions, run:

   ```bash
   pnpm publish
   ```

### Important Notes

- Add an npm token as a GitHub secret if using GitHub Actions for automated publishing.
- In the GitHub repository settings, enable **"Read & write permissions"** under **Actions** to ensure workflows run smoothly.

Once complete, `react-simple-devicons` will be live on npm!
