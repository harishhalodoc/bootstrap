---
layout: docs
title: Opacity
description: Control the opacity of elements, with opacity utilities.
group: utilities
---

The `opacity` property sets the opacity level for an element. The opacity level describes the transparency level, where 1 is not transparent at all, 0.5 is 50% visible, and 0 is completely transparent.

Set the `opacity` of an element using `.opacity-{value}` utilities.

## Examples

{{< example >}}
<div class="d-flex flex-wrap">
  <div class="opacity-100 p-3 m-2 bg-primary text-light fw-bold rounded">100%</div>
  <div class="opacity-75 p-3 m-2 bg-primary text-light fw-bold rounded">75%</div>
  <div class="opacity-50 p-3 m-2 bg-primary text-light fw-bold rounded">50%</div>
  <div class="opacity-25 p-3 m-2 bg-primary text-light fw-bold rounded">25%</div>
</div>
{{< /example >}}

Responsive variations also exist for `opacity`.

{{< markdown >}}
{{< opacity.inline >}}
{{- range $.Site.Data.breakpoints }}
- `.opacity{{ .abbr }}-0`
{{- end -}}
{{- range $.Site.Data.breakpoints }}
- `.opacity{{ .abbr }}-25`
{{- end -}}
{{- range $.Site.Data.breakpoints }}
- `.opacity{{ .abbr }}-50`
{{- end -}}
{{- range $.Site.Data.breakpoints }}
- `.opacity{{ .abbr }}-75`
{{- end -}}
{{- range $.Site.Data.breakpoints }}
- `.opacity{{ .abbr }}-100`
{{- end -}}
{{< /opacity.inline >}}
{{< /markdown >}}

### Utilities API

Opacity utilities are declared in our utilities API in `scss/_utilities.scss`. [Learn how to use the utilities API.]({{< docsref "/utilities/api#using-the-api" >}})

{{< scss-docs name="utils-opacity" file="scss/_utilities.scss" >}}
