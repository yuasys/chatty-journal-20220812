# chatty-journal-20220812
## このリポジトリについて

### Githubのmdファイル描画は、癖が強すぎ！（今日発見したこと）

<details>
<summary><label style="font-size:1.2rem">事例１ : 文字色指定に対する振る舞い</label></summary>
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
<summary><label style="font-size:1.2rem">事例２ : サマリー表示の振る舞い</label></summary>
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
<img src='./images/fig002.png' style="width:160px">|<img src='./images/fig001.png' style="width:160px">|Githubは無視する<br/>対応策はない模様

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

<details>
  <!-- ブロック要素h2でラップして（包んで）あることに留意 -->
<summary><div> <h2>サマリーです</h2> </summary>
 <h3>タイトル</h3>
 <p>詳細ブロックの本文</p>
</details>
