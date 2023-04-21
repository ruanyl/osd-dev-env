## Onboarding plugins

1. Update `artifacts.json` to add the plugin or update the url of the plugin

2. Specify the plugin `name` and `url`:
```json
{
  "name": "mlCommonsDashboards",
  "url": "https://url.to.plugin.zip"
}
```

The url should be publicly accessible, we will pull the plugin zip and persist it as the repo release assets.
So it doesn't matter if the url only valid for a short while, as long as it's been persisted, the url will be
updated automatically to the persisted url.

The `name` should match the name that user can used with `opensearch-dashboards-plugin install <name>` if it's an officially released plugin.
If it's a new plugin which hasn't released yet, you can choose a name you like.

Example opensearch plugin name:
```
alertingDashboards
anomalyDetectionDashboards
customImportMapDashboards
ganttChartDashboards
indexManagementDashboards
mlCommonsDashboards
notificationsDashboards
observabilityDashboards
queryWorkbenchDashboards
reportsDashboards
searchRelevanceDashboards
securityAnalyticsDashboards
securityDashboards
```
