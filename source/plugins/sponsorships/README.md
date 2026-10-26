<!--header-->
<table>
  <tr><td colspan="2"><a href="/README.md#-plugins">← Back to plugins index</a></td></tr>
  <tr><th colspan="2"><h3>💝 GitHub Sponsorships</h3></th></tr>
  <tr><td colspan="2" align="center"><p>This plugin displays sponsorships funded through <a href="https://github.com/sponsors/">GitHub sponsors</a>.</p>
</td></tr>
  <tr><th>⚠️ Disclaimer</th><td><p>This plugin is not affiliated, associated, authorized, endorsed by, or in any way officially connected with <a href="https://github.com">GitHub</a>.
All product and company names are trademarks™ or registered® trademarks of their respective holders.</p>
</td></tr>
  <tr>
    <th rowspan="3">Supported features<br><sub><a href="metadata.yml">→ Full specification</a></sub></th>
    <td><a href="/source/templates/classic/README.md"><code>📗 Classic template</code></a></td>
  </tr>
  <tr>
    <td><code>👤 Users</code> <code>👥 Organizations</code></td>
  </tr>
  <tr>
    <td><code>🔑 read:user</code> <code>🔑 read:org</code> <code>read:packages (optional)</code> <code>repo (optional)</code></td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <img src="https://github.com/mrDuckdevX/matrix-duck/blob/examples/metrics.plugin.sponsorships.svg" alt=""></img>
      <img width="900" height="1" alt="">
    </td>
  </tr>
</table>
<!--/header-->

## ➡️ Available options

<!--options-->
<table>
  <tr>
    <td align="center" nowrap="nowrap">Option</i></td><td align="center" nowrap="nowrap">Description</td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_sponsorships</code></h4></td>
    <td rowspan="2"><p>Enable sponsorships plugin</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>boolean</code>
<br>
<b>default:</b> no<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_sponsorships_sections</code></h4></td>
    <td rowspan="2"><p>Displayed sections</p>
<ul>
<li><code>amount</code>: display total amount sponsored</li>
<li><code>sponsorships</code>: display GitHub sponsorships</li>
</ul>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>array</code>
<i>(comma-separated)</i>
<br>
<b>default:</b> amount, sponsorships<br>
<b>allowed values:</b><ul><li>amount</li><li>sponsorships</li></ul></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_sponsorships_size</code></h4></td>
    <td rowspan="2"><p>Profile picture display size</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(8 ≤
𝑥
≤ 64)</i>
<br>
<b>default:</b> 24<br></td>
  </tr>
</table>
<!--/options-->

## ℹ️ Examples workflows

<!--examples-->
```yaml
name: 💝 GitHub Sponsorships
uses: mrDuckdevX/matrix-duck@latest
with:
  filename: metrics.plugin.sponsorships.svg
  token: ${{ secrets.METRICS_TOKEN_PERSONAL }}
  base: ""
  plugin_sponsorships: yes

```
<!--/examples-->
