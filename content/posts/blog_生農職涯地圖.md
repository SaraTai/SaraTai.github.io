---
title: "生農院求職焦慮地圖"
date: 2022-11-17T01:59:22+08:00
# weight: 1
# aliases: ["/first"]
tags: []
categories: ["Blog"]
showToc: true
TocOpen: true
draft: true
hidemeta: false
comments: true
description: "生農仔站出來"
canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: true
disableHLJS: false
hideSummary: true
searchHidden: false
ShowReadingTime: false
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: false
ShowRssButtonInSectionTermList: true
UseHugoToc: true
mermaid: true
cover:
    image: "<image path/url>" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
{{ if .Page.Store.Get "hasMermaid" }}
  <script src="https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js"></script>
  <script>
    mermaid.initialize({ startOnLoad: true });
  </script>
{{ end }}
---
{{< mermaid >}}
sequenceDiagram
    participant 育種
    participant 生產
    participant 加工
    participant 銷售
    育種->>生產: Hello John, how are you?
    loop Healthcheck
        生產->>生產: Fight against hypochondria
    end
    Note right of 加工: Rational thoughts <br/>prevail!
    生產-->>育種: Great!
    生產->>銷售: How about you?
    銷售-->>生產: Jolly good!
{{< /mermaid >}}

{{ if (.Params.mermaid) }}
<!-- MermaidJS support -->
<script async src="https://unpkg.com/mermaid@8.2.3/dist/mermaid.min.js"></script>
{{ end }}
{{ if .Page.Store.Get "hasMermaid" }}
  <script src="https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js"></script>
  <script>
    mermaid.initialize({ startOnLoad: true });
  </script>
{{ end }}