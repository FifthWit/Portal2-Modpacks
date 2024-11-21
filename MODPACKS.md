# Modpacks

Modpacks are our in-house system for managing custom modpacks from the [Modpacks repository](https://github.com/FifthWit/Portal2-Modpacks).

## Creating a Custom Modpack

Create a `modpack.manifest.json` file, place it in the root, e.g. `/portal2_dlc/modpack.manifest.json` of your modpack folder. The manifest file must include the following fields: `title`, `game`, and `category`.

### Manifest File Structure

```json
{
  "title": "string",
  "category": "string",
  "game": "string",
  "description": "string | null",
  "author": "string | null",
  "license": "string | null",
  "source": "string | null",
  "version": "string | null"
}
```

| Field         | Type             | Description                                                             |
| ------------- | ---------------- | ----------------------------------------------------------------------- |
| `title`       | `string`         | Title of the modpack                                                    |
| `category`    | `string`         | Purpose of the modpack, e.g., UI, speedrunning, cosmetic, etc.          |
| `game`        | `string`         | Game the modpack is intended for, like `Portal 2`, `Portal Revolution`  |
| `description` | `string`, `null` | Description of your modpack                                             |
| `author`      | `string`, `null` | Author of your modpack                                                  |
| `license`     | `string`, `null` | Licensing for your modpack                                              |
| `source`      | `string`, `null` | Source of your modpack, e.g., if you have a GitHub repo, it's hosted at |
| `version`     | `string`, `null` | Version of your modpack, useful for adding programmatic updates         |
