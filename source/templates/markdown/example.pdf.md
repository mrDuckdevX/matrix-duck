# 📒 Markdown template example (pdf)

See [rendering of this file here](https://github.com/mrDuckdevX/matrix-duck/blob/examples/metrics.markdown.pdf) and [original template source here](https://github.com/mrDuckdevX/matrix-duck/blob/main/source/templates/markdown/example.pdf.md).

## 🧩 Plugins

All markdown features are supported, meaning that both markdown plugins and SVG renders can be used.

<%- await include(`partials/rss.ejs`) %>

<%- await embed(`example-isocalendar-pdf`, {isocalendar:true}) %>
