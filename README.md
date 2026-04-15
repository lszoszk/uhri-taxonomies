# UHRI Taxonomies

Community-contributed taxonomies for classifying UN human rights recommendations.

Each taxonomy is a JSON file containing:
- **Categories** — the topics/labels to tag recommendations with
- **Tagged examples** — sample recommendations with human-assigned labels, useful for training classifiers

## How to use

1. Open the [UN Human Rights Analytics Dashboard](https://lszoszk.github.io/uhri-dashboard/dashboard-codex-pages/)
2. Click **Open Labeling Tool**
3. In Step 1, click **Browse community taxonomies**
4. Select a taxonomy — categories and tagged examples load automatically

## How to contribute

1. In the dashboard's Labeling Tool, define your categories and tag some records
2. Click **Share this taxonomy** in Step 3
3. Download the JSON file and [open a Pull Request](../../pulls) adding it to the `taxonomies/` folder
4. Or [create an Issue](../../issues/new?template=new-taxonomy.md) and attach your JSON file

## Taxonomy format

```json
{
  "id": "my-taxonomy",
  "name": "My Taxonomy",
  "author": "Your Name",
  "description": "What this taxonomy covers and when to use it",
  "categories": ["Category A", "Category B"],
  "examples": [
    {
      "text": "The Committee recommends that...",
      "labels": ["Category A"]
    }
  ]
}
```

## Available taxonomies

| Name | Categories | Examples | Author |
|------|-----------|----------|--------|
| [Rule of Law (Venice Commission)](taxonomies/rule-of-law.json) | 6 | 30 | HURIDOCS |

## License

Taxonomies are shared under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) unless otherwise noted.
