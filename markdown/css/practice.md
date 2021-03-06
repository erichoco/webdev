側欄
----
想要做的[目標網頁](http://www.csszengarden.com/?cssfile=001/001.css)

<p class="fragment">`.sidebar` 固定在右邊 → 將它自 normal flow 中拿出來。</p>
<div class="fragment">

  <p>兩種從 normal flow 拿出的方法：</p>

  <ul>
    <li>Absolute positioning: 設置 `position: absolute`</li>
    <li>float: 設置 `float: right`</li>
  </ul>

  `position: fixed` 與 `float: left` 不適用於這裡。

</div>

---

側欄（續）
--------

左欄（`.intro` 與 `.main`）隨視窗大小而動

<ul class="fragment">
  <li>
    若 `.sidebar` 使用 `float: right`<br>
     → 左欄什麼都不用設（留在 normal flow 中）<br>
     注意若左欄較 .sidebar 長，那麼會變這樣 →
     <img src="images/css/column.jpg" alt="float: right" style="vertical-align: -130px;">
  </li>
  <li>若使用 `position: absolute`<br>
    → 左欄須設 `padding-right` (不然左欄會和 .sidebar 疊在一起)<br>
    [範例結果](sample/css/zengarden.html)（[範例 CSS 檔](sample/css/zengarden.css)）
  </li>
</ul>

---

下拉式選單
--------

[範例結果](sample/css/menu.html)（[範例 CSS 檔](sample/css/menu.css)）

<ul>
  <li class="fragment">橫向排列的 `li` 元素<br>
    <ul>
      <li>可以用 `float`</li>
      <li>可以用 `display: inline-block`</li>
    </ul>
  </li>
  <li class="fragment">巢狀 list: `<li>` 裡可以有 `<ul>`</li>
  <li class="fragment">`:hover` magic</li>
</ul>
