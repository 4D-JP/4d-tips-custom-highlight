# 4d-tips-custom-highlight
リストフォームのハイライトカラーをカスタマイズする簡単な例題

###出来上がりのイメージ

<img width="576" alt="c" src="https://cloud.githubusercontent.com/assets/10509075/23646839/065337f0-0356-11e7-9aea-2a21956506e2.png">

###解説

リストフォームの行を選択したときのハイライトカラーは，システムで設定された値を継承しています。

[OBJECT SET RGB COLORS ](http://doc.4d.com/4Dv15/4D/15.4/OBJECT-SET-RGB-COLORS.301-3273836.ja.html)

<img width="576" alt="a" src="https://cloud.githubusercontent.com/assets/10509075/23646840/0673d320-0356-11e7-82e5-543cc9ba8ca0.png">

実際には，背景色（通常はホワイト）とシステムのリスト強調色を『混ぜた』色が使われます。一般的にリスト強調色はブルー（非アクティブウィンドウであればグレー）ですので，背景色を赤に設定すると，選択した行がパープルまたはピンクで表示されるようになります。

<img width="576" alt="b" src="https://cloud.githubusercontent.com/assets/10509075/23646838/0650d78a-0356-11e7-9ef5-5f22c64c4ea1.png">

しかしこれでは，選択されていない行の背景色が派手すぎ・・・

リストフォームをデザインモードで開き，背景オブジェクト（白い四角形）を選択して『表示』プロパティ（デフォルトは『常に表示』）を『レコード非選択時』に変更します。

同じオブジェクトを複製（``Control``+``D``）し，色を赤に変更してから，『表示』プロパティを『レコード選択時』に変更します。

これだけで，リストフォームのハイライトカラーをカスタマイズすることができます。

###参考

16R2では，__リストボックス__のハイライト表示そのものをオフにすることができるようになりました。（``LISTBOX SET PROPERTY``+``lk hide selection highlight``）

http://doc.4d.com/4Dv16R2/4D/16-R2.1620/LISTBOX-SET-PROPERTY.301-3125266.ja.html

ハイライト表示をオフにすることにより，選択された行に任意のハイライトカラーを適用することができます。

http://blog.4d.com/listbox-more-programming-possibilities/
