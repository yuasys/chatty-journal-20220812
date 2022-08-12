# chatty-journal-20220812
## 今日の気づき

<details></br>
<summary><h3 style="display:inline">Githubのmdファイル描画は、癖が強すぎ！（今日発見したこと）</h3></summary>
<div style="width:100%;padding-left:2rem">
  <details>
  <summary><h4 style="display:inline">事例１ : 文字色指定に対する振る舞い</h4></summary>
  <br/>★コード

  ```html
  <p>文字色を<span style="color:red">赤く</span>する</p>
  ```
  ★結果<br>

  Github|そのほか|メモ(対応策など)
  ----|----|----
  <img src='./images/fig002.png' style="width:160px">|<img src='./images/fig001.png' style="width:160px">|Githubは無視する<br/>対応策はない模様

  </details>


  <details>
  <summary><h4 style="display:inline">事例２ : サマリー表示の振る舞い</h4></summary>
  <br/>★コード

  ```html
  <details>
    <!-- ブロック要素h2でラップして（包んで）あることに留意 -->
  <summary><div> <h2>サマリーです</h2> </summary>
  <h3>タイトル</h3>
  <p>詳細ブロックの本文</p>
  </details>
  ```
  ★結果<br>

  Github|そのほか|メモ(対応策など)
  ----|----|----
  <img src='./images/fig003.png' style="width:160px">|<img src='./images/fig004.png' style="width:160px">|Githubはブロック要素をインライン要素とみなしてふるまう。<br/><br/>【対応策】ブロック要素の属性に<code>syle="display:inline"</code>を<br/>挿入して表示を統一する。

  </details>
</div>
</details>
<hr/>
<details>
<summary>アコーディオンひな形</summary>
 <h3>タイトル</h3>
 <ol>
  <li>番号付きリスト</li>
  <li></li>
 </ol>
 <ul>
  <li>記号付きリスト</li>
  <li></li>
 </ul>
</details>

<hr/>
