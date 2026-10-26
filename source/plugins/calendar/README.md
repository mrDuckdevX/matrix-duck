<!--header-->
<table>
  <tr><td colspan="2"><a href="/README.md#-plugins">← Back to plugins index</a></td></tr>
  <tr><th colspan="2"><h3>📆 Commit calendar</h3></th></tr>
  <tr><td colspan="2" align="center"><p>This plugin can display commit calendar across several years.</p>
</td></tr>
  <tr><th>⚠️ Disclaimer</th><td><p>This plugin is not affiliated, associated, authorized, endorsed by, or in any way officially connected with <a href="https://github.com">GitHub</a>.
All product and company names are trademarks™ or registered® trademarks of their respective holders.</p>
</td></tr>
  <tr>
    <th rowspan="3">Supported features<br><sub><a href="metadata.yml">→ Full specification</a></sub></th>
    <td><a href="/source/templates/classic/README.md"><code>📗 Classic template</code></a></td>
  </tr>
  <tr>
    <td><code>👤 Users</code></td>
  </tr>
  <tr>
    <td><code>🔑 (scopeless)</code> <code>read:org (optional)</code> <code>read:user (optional)</code> <code>read:packages (optional)</code> <code>repo (optional)</code></td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <details><summary>Current year</summary><img src="https://github.com/mrDuckdevX/matrix-duck/blob/examples/metrics.plugin.calendar.svg" alt=""></img></details>
      <details open><summary>Full history</summary><img src="https://github.com/mrDuckdevX/matrix-duck/blob/examples/metrics.plugin.calendar.full.svg" alt=""></img></details>
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
    <td nowrap="nowrap"><h4><code>plugin_calendar</code></h4></td>
    <td rowspan="2"><p>Enable calendar plugin</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>boolean</code>
<br>
<b>default:</b> no<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_calendar_limit</code></h4></td>
    <td rowspan="2"><p>Years to display</p>
<p>This option has different behaviours depending on its value:</p>
<ul>
<li><code>n &gt; 0</code> will display the last <code>n</code> years, relative to current year</li>
<li><code>n == 0</code> will display all years starting from GitHub account registration date</li>
<li><code>n &lt; 0</code> will display all years plus <code>n</code> additional years, relative to GitHub account registration date<ul>
<li>Use this when there are commits pushed before GitHub registration</li>
</ul>
</li>
</ul>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<br>
<b>zero behaviour:</b> disable</br>
<b>default:</b> 1<br></td>
  </tr>
</table>
<!--/options-->

## ℹ️ Examples workflows

<!--examples-->
```yaml
name: Current year calendar
uses: mrDuckdevX/matrix-duck@latest
with:
  filename: metrics.plugin.calendar.svg
  token: ${{ secrets.METRICS_TOKEN }}
  base: ""
  plugin_calendar: yes

```
```yaml
name: Full history calendar
uses: mrDuckdevX/matrix-duck@latest
with:
  filename: metrics.plugin.calendar.full.svg
  token: ${{ secrets.METRICS_TOKEN }}
  base: ""
  plugin_calendar: yes
  plugin_calendar_limit: 0

```
<!--/examples-->
