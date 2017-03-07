# 4d-tips-custom-highlight
リストフォームのハイライトカラーをカスタマイズする簡単な例題

出来上がりのイメージ

<img width="576" alt="c" src="https://cloud.githubusercontent.com/assets/10509075/23646839/065337f0-0356-11e7-9aea-2a21956506e2.png">

###解説

リストフォームの行を選択したときのハイライトカラーは，システムで設定された値を継承しています。

[OBJECT SET RGB COLORS ](http://doc.4d.com/4Dv15/4D/15.4/OBJECT-SET-RGB-COLORS.301-3273836.ja.html)

実際には，背景色（通常はホワイト）とシステムのリスト強調色を『混ぜた』色が使われます。一般的にリスト強調色はブルー（非アクティブウィンドウであればグレー）ですので，背景色を赤に設定すると，選択した行がパープルまたはピンクで表示されるようになります。

<img width="576" alt="a" src="https://cloud.githubusercontent.com/assets/10509075/23646840/0673d320-0356-11e7-82e5-543cc9ba8ca0.png">

<img width="576" alt="b" src="https://cloud.githubusercontent.com/assets/10509075/23646838/0650d78a-0356-11e7-9ef5-5f22c64c4ea1.png">
