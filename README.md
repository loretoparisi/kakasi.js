# kakasi.js
Kakasi Japanese Transliteration for Node.js

## Usage
```bash
git clone https://github.com/loretoparisi/kakasi.js.git
cd kakasi.js/examples
node transliterate.js 
deakubibakkashiteita 
```

## How to use kakasi.js
### Transliterate
```javascript
var documents = [
        "退屈であくびばっかしていた毎日\n想像を超えた君が変えてゆく\nいつからかチラ見してる 斜め後ろからはちきれそうな胸の高鳴り\n\n不思議な力 気づけば追いかけてしまう\nなんてこった！これってとんだΨ難(さいなん)？\n\n恋、弾けました。\n止まらないんです 寝ても覚めても君が\n溢れ出した トキメキに戸惑ってるんだ\n読み取れない心模様 振り向いてテレパシー\n見たこともないセカイ 君と\n\n最近ため息ばっか らしくないけど\n想像しちゃう君とのあれこれ\n\n驚くばかり 知るほどに振り回されてる\nてんやわんや でもちょっと快感\n\n恋、弾けました。\n浮かんでくるよ なにをしてても君が\n人前でニヤけそうで ごまかしてるんだ\n駆け出したい今すぐに 連れてってテレポーテーション\nどんな未来がきても 君と\n\nインスタに投稿(アップ)している エフェクト越しの写真よりも\n目の前にいる君の方が 1000万倍魅力的だ\n\nねえ 君はもしや超能力者？\nこんな夢中にさせて 見つめ合えば動けないんだ\nハートが聞こえそう\n\n恋、弾けました。\n止まらないんです 寝ても覚めても君が\n溢れ出した トキメキに戸惑ってるんだ\n読み取れない心模様 振り向いてテレパシー\n見たこともないセカイ どんな未来がきても\n恋は宇宙(そら)へ飛んでゆく 君と"
    ];
    
var kk = new Kakasi({
    debug: false
});
kk.transliterate( "退屈であくびばっかしていた毎日" )
.then(results => {
    console.log("----------\n%s\n----------",results);
})
.catch(error => {
    console.error(error);
});
```

this will end up in `taikutsu deakubibakkashiteita mainichi`

