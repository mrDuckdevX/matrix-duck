<!--header-->
<table>
  <tr><td colspan="2"><a href="/README.md#-plugins">← Back to plugins index</a></td></tr>
  <tr><th colspan="2"><h3>♟️ Chess</h3></th></tr>
  <tr><td colspan="2" align="center"><p>This plugin displays the last game you played on a supported chess platform.</p>
</td></tr>
  <tr><th>⚠️ Disclaimer</th><td><p>This plugin is not affiliated, associated, authorized, endorsed by, or in any way officially connected with any of the supported provider.
All product and company names are trademarks™ or registered® trademarks of their respective holders.</p>
</td></tr>
<tr><th>Authors</th><td><a href="https://github.com/matrix-duck">@matrix-duck</a></td></tr>
  <tr>
    <th rowspan="3">Supported features<br><sub><a href="metadata.yml">→ Full specification</a></sub></th>
    <td><a href="/source/templates/classic/README.md"><code>📗 Classic template</code></a></td>
  </tr>
  <tr>
    <td><code>👤 Users</code> <code>👥 Organizations</code> <code>📓 Repositories</code></td>
  </tr>
  <tr>
    <td><code>🗝️ plugin_chess_token</code></td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <img src="https://github.com/mrDuckdevX/matrix-duck/blob/examples/metrics.plugin.chess.svg" alt=""></img>
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
    <td nowrap="nowrap"><h4><code>plugin_chess</code></h4></td>
    <td rowspan="2"><p>Enable chess plugin</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>boolean</code>
<br>
<b>default:</b> no<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_chess_token</code></h4></td>
    <td rowspan="2"><p>Chess platform token</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap">🔐 Token<br>
🌐 Web instances must configure <code>settings.json</code>:
<ul>
<li><i>metrics.api.chess.any</i></li>
</ul>
<b>type:</b> <code>token</code>
<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_chess_user</code></h4></td>
    <td rowspan="2"><p>Chess platform login</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap">⏯️ Cannot be preset<br>
<b>type:</b> <code>string</code>
<br>
<b>default:</b> <code>→ User login</code><br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_chess_platform</code></h4></td>
    <td rowspan="2"><p>Chess platform</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>string</code>
<br>
<b>allowed values:</b><ul><li>lichess.org</li></ul></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_chess_animation</code></h4></td>
    <td rowspan="2"><p>Animation settings</p>
<ul>
<li><code>size</code> is the size of a single chessboard square in pixels (board will be 8 times larger)</li>
<li><code>delay</code> is the delay before starting animation (in seconds)</li>
<li><code>duration</code> is the duration of the animation of a move (in seconds)</li>
</ul>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>json</code>
<br>
<b>default:</b> <details><summary>→ Click to expand</summary><pre language="json"><code>{
  "size": 40,
  "delay": 3,
  "duration": 0.6
}
</code></pre></details><br></td>
  </tr>
</table>
<!--/options-->

## 🗝️ Obtaining a lichess.org token

Create a [lichess.org account](https://lichess.org) and select [API access tokens](https://lichess.org/account/oauth/token) to get a token.

![lichess.org token](/.github/readme/imgs/plugin_chess_lichess_token_0.png)

It is not necessary to add additional scopes:

![lichess.org token](/.github/readme/imgs/plugin_chess_lichess_token_1.png)

Create token and store it in your secrets:

![lichess.org token](/.github/readme/imgs/plugin_chess_lichess_token_0.png)

## ℹ️ Examples workflows

<!--examples-->
```yaml
name: Last chess game from lichess.org
uses: mrDuckdevX/matrix-duck@latest
with:
  filename: metrics.plugin.chess.svg
  token: NOT_NEEDED
  base: ""
  plugin_chess: yes
  plugin_chess_token: ${{ secrets.CHESS_TOKEN }}
  plugin_chess_platform: lichess.org

```
<!--/examples-->
