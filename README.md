# ditto-helm-chart
Helm Chart Repo for Eclipse Ditto

## Submodules

This repository contains a submodule with the source code of the packages. To clone the repository with all submodules, use:

```bash
git clone --recurse-submodules -j8 git@github.com:ATNoG/ditto-helm-chart.git
cd ditto-helm-chart
```

## Add/Edit chart to the repo

1. Package the chart

```bash
helm package <chart-name>
```

2. Move the packaged chart to the repo /charts directory

```bash
mv <chart-name>.tgz charts/
```

3. Update the index.yaml

```bash
helm repo index . --url https://ATNoG.github.io/ditto-helm-chart
```

4. Commit and push the changes

## Run the chart

helm install -n cloud2edge -f <values.yaml> c2e https://atnog.github.io/ditto-helm-chart/cloud2edge
