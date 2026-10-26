<!--header-->
<table>
  <tr><td colspan="2"><a href="/README.md#-plugins">← Back to plugins index</a></td></tr>
  <tr><th colspan="2"><h3>📓 Featured repositories</h3></th></tr>
  <tr><td colspan="2" align="center"><p>This plugin displays a list of chosen featured repositories.</p>
<p>Since it is possible to <a href="https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/pinning-items-to-your-profile">pin repositories</a> on GitHub, this plugin is mostly intended for external usage.</p>
</td></tr>
  <tr><th>⚠️ Disclaimer</th><td><p>This plugin is not affiliated, associated, authorized, endorsed by, or in any way officially connected with <a href="https://github.com">GitHub</a>.
All product and company names are trademarks™ or registered® trademarks of their respective holders.</p>
</td></tr>
  <tr><th>ℹ Additional notes</th><td><blockquote>
<p>⚠️ Due to limitations of using SVG images inside <code>&lt;img&gt;</code> tags, clicking on a repository card will not redirect to repository page.</p>
</blockquote>
</td></tr>
  <tr>
    <th rowspan="3">Supported features<br><sub><a href="metadata.yml">→ Full specification</a></sub></th>
    <td><a href="/source/templates/classic/README.md"><code>📗 Classic template</code></a></td>
  </tr>
  <tr>
    <td><code>👤 Users</code> <code>👥 Organizations</code></td>
  </tr>
  <tr>
    <td><code>🔑 (scopeless)</code> <code>read:org (optional)</code> <code>read:user (optional)</code> <code>read:packages (optional)</code> <code>repo (optional)</code></td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <details open><summary>Featured</summary><img src="https://github.com/mrDuckdevX/matrix-duck/blob/examples/metrics.plugin.repositories.svg" alt=""></img></details>
      <details><summary>Pinned</summary><img src="https://github.com/mrDuckdevX/matrix-duck/blob/examples/metrics.plugin.repositories.pinned.svg" alt=""></img></details>
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
    <td nowrap="nowrap"><h4><code>plugin_repositories</code></h4></td>
    <td rowspan="2"><p>Enable repositories plugin</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>boolean</code>
<br>
<b>default:</b> no<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_repositories_featured</code></h4></td>
    <td rowspan="2"><p>Featured repositories</p>
<p>Current <a href="/source/plugins/core/README.md#user"><code>user</code></a> will be used when no owner is specified</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap">⏯️ Cannot be preset<br>
<b>type:</b> <code>array</code>
<i>(comma-separated)</i>
<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_repositories_pinned</code></h4></td>
    <td rowspan="2"><p>Pinned repositories</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(0 ≤
𝑥
≤ 6)</i>
<br>
<b>default:</b> 0<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_repositories_starred</code></h4></td>
    <td rowspan="2"><p>Featured most starred repositories</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(0 ≤
𝑥
≤ 100)</i>
<br>
<b>default:</b> 0<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_repositories_random</code></h4></td>
    <td rowspan="2"><p>Featured random repositories</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(0 ≤
𝑥
≤ 100)</i>
<br>
<b>default:</b> 0<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_repositories_order</code></h4></td>
    <td rowspan="2"><p>Featured repositories display order</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>array</code>
<br>
<b>default:</b> featured, pinned, starred, random<br>
<b>allowed values:</b><ul><li>featured</li><li>pinned</li><li>starred</li><li>random</li></ul></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_repositories_forks</code></h4></td>
    <td rowspan="2"><p>Include repositories forks</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>boolean</code>
<br>
<b>default:</b> no<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_repositories_affiliations</code></h4></td>
    <td rowspan="2"><p>Repositories affiliations</p>
<ul>
<li><code>owner</code>: owned repositories</li>
<li><code>collaborator</code>: repositories with push access</li>
<li><code>organization_member</code>: repositories from an organization where user is a member</li>
</ul>
<p>Set to <code>&quot;&quot;</code> to disable and fetch all repositories related to given account.</p>
<p>This option changes which repositories will be fetched by <a href="/source/plugins/projects/README.md#plugin_repositories_starred"><code>plugin_repositories_starred</code></a> and <a href="/source/plugins/projects/README.md#plugin_repositories_random"><code>plugin_repositories_random</code></a> options</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>array</code>
<i>(comma-separated)</i>
<br>
<b>default:</b> owner<br>
<b>allowed values:</b><ul><li>owner</li><li>collaborator</li><li>organization_member</li></ul></td>
  </tr>
</table>
<!--/options-->

## ℹ️ Examples workflows

<!--examples-->
```yaml
name: Featured repositories
uses: mrDuckdevX/matrix-duck@latest
with:
  filename: metrics.plugin.repositories.svg
  token: ${{ secrets.METRICS_TOKEN }}
  base: ""
  plugin_repositories: yes
  plugin_repositories_featured: mrDuckdevX/matrix-duck

```
```yaml
name: Pinned repositories
uses: mrDuckdevX/matrix-duck@latest
with:
  filename: metrics.plugin.repositories.pinned.svg
  token: ${{ secrets.METRICS_TOKEN }}
  base: ""
  plugin_repositories: yes
  plugin_repositories_pinned: 2

```
<!--/examples-->
