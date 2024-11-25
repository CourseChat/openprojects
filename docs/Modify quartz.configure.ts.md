TOC

Let me help explain how to create a table of contents (TOC) for a folder in Obsidian using Quartz. 

First, it's important to understand that this involves modifying the Quartz configuration file to generate a TOC based on your Obsidian vault's folder structure. Here's how:

1. In your Quartz directory, locate the `/quartz.config.ts` file. This is where you'll configure the folder-based TOC.

2. You'll use the `Plugin.ContentPage` and `Plugin.Folders` plugins to set this up. Here's the relevant code you would add:

```typescript
import { QuartzConfig } from "./quartz/cfg"
import * as Component from "./quartz/components"

const config: QuartzConfig = {
  configuration: {
    // ... other config options ...
    plugins: {
      transformers: [
        Plugin.FrontMatter(),
        Plugin.TableOfContents({
          collapseByDefault: false, // Set to true if you want the TOC collapsed initially
          showByDefault: true,
        }),
        Plugin.Folders({
          folderDefaultState: "collapsed", // or "open"
          folderClickBehavior: "collapse", // or "link"
        }),
      ],
      // ... other plugins ...
    },
  },
}

export default config
```

3. For any folder where you want a TOC, create an `index.md` file in that folder. In this file, you can use the following syntax:

```markdown
---
title: Your Folder Name
enableToc: true
---

## Table of Contents
{{! folder }}
```

The `{{! folder }}` syntax tells Quartz to generate a TOC for that folder's contents.

4. If you want to customize the appearance of your TOC, you can modify the styles in your theme file (usually found in `/quartz/styles`).

Remember that:
- The TOC will automatically update when you add or remove files from the folder
- You can exclude files from the TOC by adding `excludeFromToc: true` in their frontmatter
- The hierarchy in the TOC will match your folder structure
- Links in the TOC will be formatted according to your Quartz configuration settings

You'll need to rebuild your Quartz site after making these changes by running `npx quartz build` in your terminal.

Would you like me to explain any part of this in more detail?