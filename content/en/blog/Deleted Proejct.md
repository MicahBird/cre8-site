---
author: "Not Me"
title: "Deleted Proejct"
date: 2023/03/03
description: "This is a deleted project"
tags: ["Art, Poetry, Scratch"]
thumbnail: "https://drive.google.com/open?id=15mMuj6QblYkXfjStN_n56qpEhVO6i4GL"
---

## Code Fencing

Use code fencing to highlight the syntax of a specific language.

```json
{
  "version": "0.2.0",
  "themes": [],
  "projects": [],
  "configuration": {}
}
```

```html
<div class="highlight">
    <pre>
        <code>some code...</code>
    </pre>
</div>
```

## Highlight Shortcode

Use the `highlight` shortcode to customize the layout of a specific code block.

{{< highlight go "linenos=table,hl_lines=8 15-17,linenostart=199" >}}
// GetTitleFunc returns a func that can be used to transform a string to
// title case.
//
// The supported styles are
//
// - "Go" (strings.Title)
// - "AP" (see https://www.apstylebook.com/)
// - "Chicago" (see https://www.chicagomanualofstyle.org/home.html)
//
// If an unknown or empty style is provided, AP style is what you get.
func GetTitleFunc(style string) func(s string) string {
  switch strings.ToLower(style) {
  case "go":
    return strings.Title
  case "chicago":
    return transform.NewTitleConverter(transform.ChicagoStyle)
  default:
    return transform.NewTitleConverter(transform.APStyle)
  }
}
{{< / highlight >}}