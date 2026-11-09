# ForgeHub

ForgeHub is a responsive, static Minecraft mod discovery and sharing website for GitHub Pages. It includes a searchable catalog, category and loader filters, sorting, project details, favorites, theme switching, and a creator submission form.

## Publish with GitHub Pages

In **Settings → Pages**, choose **Deploy from a branch**, select `main` and the `/(root)` folder, then save. The site entry point is the root `index.html`.

## Catalog

Edit [`mods.json`](./mods.json) to add or update projects. Each catalog entry can include:

- `id`, `name`, `author`, `description`
- `category`, `loader`, `minecraft` (array), and `tags` (array)
- `rating`, `downloads`, and optional `featured: true`
- `url` for the official project/download page and optional `image` URL

The included listings are examples that link to the projects' Modrinth pages. Keep download links pointed to trusted project sources.

## Creator submissions and limitations

The submission form saves entries to the current browser's local storage; it does not upload files or publish content to the shared catalog. Use **Export my submissions** and merge the exported entries into `mods.json` to publish them. GitHub Pages serves static files and cannot securely provide user accounts, moderation, persistent public uploads, or a backend database. Those features need a server or a service such as a hosted database/API, plus authentication and moderation controls.
