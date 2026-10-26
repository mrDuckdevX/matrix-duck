<!--header-->
<table>
  <tr><td colspan="2"><a href="/README.md#-plugins">← Back to plugins index</a></td></tr>
  <tr><th colspan="2"><h3>💉 Nightscout</h3></th></tr>
  <tr><td colspan="2" align="center"><p>This plugin displays blood sugar values from a <a href="http://nightscout.info">Nightscout</a> site.</p>
</td></tr>
  <tr><th>⚠️ Disclaimer</th><td><p>This plugin is not affiliated, associated, authorized, endorsed by, or in any way officially connected with <a href="http://nightscout.info">Nightscout</a>.
All product and company names are trademarks™ or registered® trademarks of their respective holders.</p>
</td></tr>
<tr><th>Authors</th><td><a href="https://github.com/legoandmars">@legoandmars</a></td></tr>
  <tr>
    <th rowspan="3">Supported features<br><sub><a href="metadata.yml">→ Full specification</a></sub></th>
    <td><a href="/source/templates/classic/README.md"><code>📗 Classic template</code></a></td>
  </tr>
  <tr>
    <td><code>👤 Users</code></td>
  </tr>
  <tr>
    <td><i>No tokens are required for this plugin</i></td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <img src="https://github.com/legoandmars/legoandmars/blob/master/metrics.plugin.nightscout.svg" alt=""></img>
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
    <td nowrap="nowrap"><h4><code>plugin_nightscout</code></h4></td>
    <td rowspan="2"><p>Enable nightscout plugin</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>boolean</code>
<br>
<b>default:</b> no<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_nightscout_url</code></h4></td>
    <td rowspan="2"><p>Nightscout URL</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>string</code>
<br>
<b>default:</b> https://example.herokuapp.com<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_nightscout_datapoints</code></h4></td>
    <td rowspan="2"><p>Number of datapoints shown the graph</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(0 ≤
𝑥)</i>
<br>
<b>zero behaviour:</b> disable</br>
<b>default:</b> 12<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_nightscout_lowalert</code></h4></td>
    <td rowspan="2"><p>Threshold for low blood sugar</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(0 ≤
𝑥)</i>
<br>
<b>default:</b> 80<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_nightscout_highalert</code></h4></td>
    <td rowspan="2"><p>Threshold for high blood sugar</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(0 ≤
𝑥)</i>
<br>
<b>default:</b> 180<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_nightscout_urgentlowalert</code></h4></td>
    <td rowspan="2"><p>Threshold for urgently low blood sugar</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(0 ≤
𝑥)</i>
<br>
<b>default:</b> 50<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_nightscout_urgenthighalert</code></h4></td>
    <td rowspan="2"><p>Threshold for urgently high blood sugar</p>
<img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code>
<i>(0 ≤
𝑥)</i>
<br>
<b>default:</b> 250<br></td>
  </tr>
</table>
<!--/options-->

## 🌐 Setup a Nightscout instance

The [nightscout website](http://www.nightscout.info/) details how to self-host a nightscout site.
Check out the instructions there.

## ℹ️ Examples workflows

<!--examples-->
```yaml
uses: mrDuckdevX/matrix-duck@latest
with:
  token: NOT_NEEDED
  plugin_nightscout: yes
  plugin_nightscout_url: ${{ secrets.NIGHTSCOUT_URL }}

```
<!--/examples-->
