## Onboarding plugins

1. Update `artifacts.json` to add the plugin or update the url of the plugin

2. Specify the plugin `name` and `url`:
```json
{
  "name": "opensearch-ml",
  "url": "https://url.to.plugin.zip"
}
```

The url should be publicly accessible, we will pull the plugin zip and persist it as the repo release assets.
So it doesn't matter if the url only valid for a short while, as long as it's been persisted, the url will be
updated automatically to the persisted url.

The `name` should match the name that user can used with `opensearch-plugin install <name>` if it's an officially released plugin.
If it's a new plugin which hasn't released yet, you can choose a name you like.

Example opensearch plugin name:
```
opensearch-alerting
opensearch-anomaly-detection
opensearch-asynchronous-search
opensearch-cross-cluster-replication
opensearch-geospatial
opensearch-index-management
opensearch-job-scheduler
opensearch-knn
opensearch-ml
opensearch-neural-search
opensearch-notifications
opensearch-notifications-core
opensearch-observability
opensearch-performance-analyzer
opensearch-reports-scheduler
opensearch-security
opensearch-security-analytics
opensearch-sql
```

The `url` should be a public accessible location.
