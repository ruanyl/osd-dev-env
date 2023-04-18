## Onboarding plugins

1. Create a `json` file in `plugins` folder, you can use any readable file name, for example, `ml-commons-dashboards.json`

2. Specify the plugin `name` and `url`:
```json
{
  "name": "mlCommonsDashboards",
  "url": "https://url.to.plugin.zip"
}
```

The `name` should match the name that user can used with `opensearch-dashboards-plugin install <name>` if it's an officially released plugin.
If it's a new plugin which hasn't released yet, you can choose a name you like.

The `url` should be a public accessible location.
