# Helm-charts

> Helm Chart Repository


## Usage
Once Helm is set up properly, add the repo as follows:

    helm repo add tmax-stable https://tmax-cloud.github.io/helm-charts/stable

You can set repo name as what you want instead of tmax-stable.


## Helm chart format
- example-chart/
  * [Chart.yaml](#Chart.yaml) (A YAML file containing information about the chart)
  * values.yaml       (The default configuration values for this chart)
  * charts/           (A directory containing any charts upon which this chart depends)
  * templates/        (A directory of templates that, when combined with values will generate valid Kubernetes manifest files)
  * LICENSE           (optional: A plain text file containing the license for the chart)
  * README.md         (optional: A human-readable README file)
  * requirements.yaml (optional: A YAML file listing dependencies for the chart)


#### Chart.yaml
Example of chart.yaml. Required field is marked. ([예시](./stable/helm-guestbook/Chart.yaml))
```yaml
apiVersion: Chart API version (required)   
name: Chart name (required)   
version: Chart version (required)   
description: A single-sentence description for this chart   
home: The URL of this project's home page   
maintainers:   
- name: The maintainer's name (required for each maintainer)   
  email: The maintainer's email          
  url: A URL for the maintainer     
icon: A URL of SVG or PNG image to be used as an icon   
keywords:   
- A list of keywords about this project   
```
