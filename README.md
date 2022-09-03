<script src="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/list.js/2.3.1/list.min.js"></script>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tify@0.27.0/dist/tify.css">

# Kumiko-Sato-310935.github.io
c4ljp2022チュートリアル
c4ljp2022練習用ページです。

<div id="books">
  <input class="search" placeholder="検索" />
  <button class="sort" data-sort="title">
    タイトルで並べ替え
  </button>
  <ul class="list">
    <!-- _data フォルダの books.csv からデータを取り出す -->
    {% for book in site.data.books %}
      <li>
        <!-- books.csv の title 列、 url 列をリンク先に設定 -->
        <p class="title"><a href="{{ book.url }}">{{ book.title }}</a></p>
      </li>
    {% endfor %}
  </ul>
</div>

<p><ul>お知らせ
<li>お知らせ①</li>
<li>お知らせ②</li>
 </ul>
 </p>
 <p>
![キムワイプ](https://user-images.githubusercontent.com/112713036/188251812-4d535e10-87f3-4a23-94bc-22b196e36236.jpg)
</p>

<iframe width="560" height="315" src="https://www.youtube.com/embed/_9spUxP_NwE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
remote_theme: daattali/beautiful-jekyll

<script>
var options = {
    valueNames: [ 'title' ]
};

var userList = new List('books', options);
</script>
