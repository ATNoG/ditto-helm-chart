# ditto-helm-chart
Helm Chart Repo for Eclipse Ditto

## Add/Edit chart to the repo

1. Package the chart

```bash
helm package <chart-name>
```

2. Move the packaged chart to the repo /charts directory

```bash
mv <chart-name>.tgz ditto-helm-chart/charts
```

3. Update the index.yaml

```bash
helm repo index ditto-helm-chart --url https://ATNoG.github.io/ditto-helm-chart
```

4. Commit and push the changes
