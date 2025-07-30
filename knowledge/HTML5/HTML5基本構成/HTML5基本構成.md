# 不要と言われている指定

`<meta http-equiv="X-UA-Compatible" content="IE=edge" />` はもう必要ない。  
[【HTML】head内のmeta『X-UA-Compatible:IE=edge』は不要です](https://125naroom.com/web/3507)  

```
<meta http-equiv="X-UA-Compatible" content="IE=edge" />
```

# 必要な指定

無くても動くが、ブラウザの表示モードを標準モードにする目的であったほうがいいらしい。  
[DOCTYPE宣言について](https://qiita.com/akatsuki174/items/16a2189f2845205fcf88)  

```
<!DOCTYPE html>
```

Googleはlang属性を全く見ていないらしいため、SEO的な意味合いなどでは不要。  
でも、あってもいいのではという意見も見られる。ちなみにGoogleのトップページにはlang属性が付いてる。(Google自身は見てないくせに...)  
[HTMLの言語指定 は必要？不要？　lang属性をGoogleは無視](https://schole-otium.com/blog/programming/html/lang-attribute-necessary/)  

```
<html lang="ja">
```

charsetは必要な場合と不要な場合があるらしい。  
が、現状では入れておいた方が良いのではと思う。Googleのトップページにもcharsetは入っている。  
[meta charset="UTF-8" を書く必要性があるケースとデメリット](https://blog.w0s.jp/639)  

```
<meta charset="UTF-8" />
```

viewportは必要。  

```
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

# 参考資料

[HTML5で個人的に最低限必要だと思う記述・タグまとめ。head内に何を書いておけばいいのか？](https://wemo.tech/79)  