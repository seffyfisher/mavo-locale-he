# Hebrew Mavo localisation

![mavo hebrew logo](hebrewMavo.svg)


Mavo UI translation in Hebrew
To use, simply include the plugin and then use lang="he" on your Mavo root, or the element.

For more info , look at https://mavo.io/docs/ui/#customizing-text--localization

How To use :

1. simply include the plugin and then use lang="he" on your Mavo root

```html
<div mv-app mv-plugins="locale-he" lang="he" mv-storage="local">
    <h1>מאבו - מה אפשר לעשות בכמה דקות</h1>
    לא להאמין! <span property="langs" mv-multiple>
    אפליקציות בסביבת אינטרנט - זה באמת מדהים לא סתם משפט משנות השמונים
    </span>
</div>
```

2. another easy way is just :
-copy the raw file content and paste it inside your html file inside a <script> tag (after loading mavo script)
-add to the mavo root element lang="he"
  
---

p.s.
#### the word "MAVO" in hebrew actually means : "introduction" which makes prefect sense!

some css fixes for texts that are right now hardcoded via the scss/css file

---

```css
.mv-message.mv-error::before{
  content: "😳 שומו שמיים! ";
}

.mv-message::before{
  content:"שימו לב : "
}

[mv-app] .mv-item-bar.mv-ui{
  direction:ltr;
}
```
