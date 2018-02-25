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

