# Slack Tomorrow Theme

A slack theme using dark themed colors.

# Installation

Add this code in the end of the file `index.js`, `ssb-interop.js`:
- Windows: `C:\Users\<user>\AppData\Local\slack\app-<slack-version>\resources\app.asar.unpacked\src\static\index.js`
- Windows: `C:\Users\<user>\AppData\Local\slack\app-<slack-version>\resources\app.asar.unpacked\src\static\ssb-interop.js`
```js
document.addEventListener('DOMContentLoaded', function() {
    $.ajax({
        url: 'https://raw.githubusercontent.com/cjmart11/slack-tomorrow-theme/master/custom.css',
        success: function(css) {
            $("<style></style>").appendTo('head').html(css)
        }
    });
});
```
