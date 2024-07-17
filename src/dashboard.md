---
theme: dashboard
title: Dataset dashboard
toc: false
---

# Our data


```js
const datasets = FileAttachment("./data/datasets.json").json();
const themes = FileAttachment("./data/themes.json").json();
const types = FileAttachment("./data/resources_types.json").json();
```

<!-- A shared color scale for consistency, sorted by the number of launches -->

```js
const color = Plot.scale({
  color: {
    type: "categorical",
    domain: types.map(d => d.type),
    unknown: "var(--theme-foreground-muted)"
  }
});

```

<h2>Number of dataset themes</h2>
<div class="grid grid-cols-4">
  <div class="card">
    <h2>Regions and cities</h2>
    <span class="big">${Number(themes.filter((d) => d.name === "Regions and cities")[0].value).toLocaleString("en-US")}</span>
  </div>
  <div class="card">
    <h2>Environment</h2>
    <span class="big">${Number(themes.filter((d) => d.name === "Environment")[0].value).toLocaleString("en-US")}</span>
  </div>
  <div class="card">
    <h2>Government and public sector</h2>
    <span class="big">${Number(themes.filter((d) => d.name === "Government and public sector")[0].value).toLocaleString("en-US")}</span>
  </div>
  <div class="card">
    <h2>Other</h2>
    <span class="big">${Number(themes.filter((d) => d.name !== "Government and public sector" && d.name !== "Environment" && d.name !== "Regions and cities")[0].value).toLocaleString("en-US")}</span>
  </div>
</div>



```js
function typesChart(data, {width}) {
  return Plot.plot({
    title: "Popular resource types",
    width,
    height: 300,
    marginTop: 0,
    marginLeft: 86,
    x: {label: "Type"},
    y: {percent: true,label: "Amount"},
    marks: [
        Plot.ruleY([0]),
        Plot.barY(data, 
            {
                x: "type", 
                y: "amount",
                sort: {
                    x: "-y", 
                    reverse: true
                }
            }
        )
    ]
  });
}

```

<div class="grid grid-cols-1">
  <div class="card">
    ${resize((width) => typesChart(types, {width}))}
  </div>
</div>
