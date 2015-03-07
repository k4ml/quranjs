# quranjs
JavaScript API to access Quran's verses.

# Usage
Include it in your HTML:-

```html
<script src="http://quranjs.github.io/quran.js" type="text/javascript"></script>
```

Then you can start using the API to access Quran's verses:-

```
var quran = new QuranJS();
quran.getVerse(1, 1);
// return بِسْمِ ٱللَّهِ ٱلرَّحْمَٰنِ ٱلرَّحِيمِ
quran.getRandomVerse();

// we can also switch the backend storage
// this will fetch data stored in firebase
// instead of the default data.js.
var quran = new QuranJS('google');
var quran = new QuranJS('firebase');
```

# Requirements
* No special servers for storage, just used any free services. Identified so far Google Spreadsheets and Firebase.

# Existing Implementations
* https://github.com/qzaidi/quran (nodejs)
* http://docs.globalquran.com/API:Javascript/Quran (https://github.com/GlobalQuran/site)
