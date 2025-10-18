<!--header-->
<table>
  <tr><td colspan="2"><a href="/README.md#-plugins">← Back to plugins index</a></td></tr>
  <tr><th colspan="2"><h3>🗳️ Leetcode</h3></th></tr>
  <tr>
    <td colspan="2" align="center">
      <p>This plugin displays statistics from a <a href="https://leetcode.com/u/JorgeNavarro/">LeetCode</a> account.</p>
    </td>
  </tr>
  <tr>
    <th>⚠️ Disclaimer</th>
    <td>
      <p>This plugin is not affiliated, associated, authorized, endorsed by, or in any way officially connected with <a href="https://leetcode.com">LeetCode</a>.
      All product and company names are trademarks™ or registered® trademarks of their respective holders.</p>
    </td>
  </tr>
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
      <img src="https://github.com/lowlighter/metrics/blob/examples/metrics.plugin.leetcode.svg" alt="Example LeetCode metrics"></img>
      <img width="900" height="1" alt="">
    </td>
  </tr>
</table>
<!--/header-->

## ➡️ Available options

<!--options-->
<table>
  <tr>
    <td align="center" nowrap="nowrap"><b>Option</b></td>
    <td align="center" nowrap="nowrap"><b>Description</b></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_leetcode</code></h4></td>
    <td rowspan="2"><p>Enable LeetCode plugin</p><img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>boolean</code><br><b>default:</b> no<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_leetcode_user</code></h4></td>
    <td rowspan="2"><p>LeetCode login</p><img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>string</code><br><b>default:</b> <code>→ JorgeNavarro</code><br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_leetcode_sections</code></h4></td>
    <td rowspan="2"><p>Displayed sections</p>
      <ul>
        <li><code>solved</code> – Display solved problems scores</li>
        <li><code>skills</code> – Display solved problems tagged skills</li>
        <li><code>recent</code> – Display recent submissions</li>
      </ul>
      <img width="900" height="1" alt="">
    </td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>array</code> <i>(comma-separated)</i><br><b>default:</b> solved<br><b>allowed values:</b> <ul><li>solved</li><li>skills</li><li>recent</li></ul></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_leetcode_limit_skills</code></h4></td>
    <td rowspan="2"><p>Display limit (skills)</p><img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code><i>(0 ≤ 𝑥)</i><br><b>default:</b> 10<br></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><h4><code>plugin_leetcode_limit_recent</code></h4></td>
    <td rowspan="2"><p>Display limit (recent)</p><img width="900" height="1" alt=""></td>
  </tr>
  <tr>
    <td nowrap="nowrap"><b>type:</b> <code>number</code><i>(1 ≤ 𝑥 ≤ 15)</i><br><b>default:</b> 5<br></td>
  </tr>
</table>
<!--/options-->
### 🧩 LeetCode Stats

[![LeetCode Stats](https://github.com/jorgenavarro13/Some_widgets/blob/master/metrics.plugin.leetcode.svg)](https://leetcode.com/u/JorgeNavarro/)


## ℹ️ Example workflow (personalized)

<!--examples-->
```yaml
- name: 🧩 LeetCode Stats
  uses: lowlighter/metrics@latest
  with:
    filename: metrics.plugin.leetcode.svg
    token: NOT_NEEDED
    base: ""
    plugin_leetcode: yes
    plugin_leetcode_user: JorgeNavarro
    plugin_leetcode_sections: solved, skills, recent
    plugin_leetcode_limit_skills: 10
    plugin_leetcode_limit_recent: 5

