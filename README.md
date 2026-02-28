# 16bit-content

Content repository for [16Bit Gallery](https://github.com/interurban/16-bit-gallery). The app loads catalog data from the `data/` JSON files via raw GitHub URLs.

## Layout

```
data/
  artworks.json
  packs.json
  artists.json
  groups.json
  tags.json
```

## Wiring the app

In the gallery app, set in `.env.local`:

```
CONTENT_REPO_URL=https://raw.githubusercontent.com/interurban/16bit-content/main
```

Then run `pnpm dev` — the app will use this repo’s data (cached 1 hour).
