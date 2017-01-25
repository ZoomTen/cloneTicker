cloneTicker
=
An HTML+JS ticker "inspired" by the web tickers a specific TV station used to give away in the mid-2000's.

Installing
-
1. Copy `cloneTicker-common.js` and `cloneTicker-categories.js` into your website's root directory.

2. Copy the folder named `tickers` (If you choose to rename it, make sure to set the `tickerbase` variable in `common.js` to the same name)

Using
-
1. In the desired webpage you want to use the cloneTickers on, add <br>`<script src="cloneTicker-common.js"></script>`<br>and **after it**,<br>`
<script src="cloneTicker-categories.js"></script>`<br>in the header.

2. Write the style to use for the tickers. Available classes are:<br>`ticker-main`, `ticker-title`, `ticker-title-generic`, and `ticker-title-*`<br>where `*` is the ID of the category. `cloneTicker.css`, the included style, should be a good enough starting style. You can use it through:<br>`<link href="cloneTicker.css" rel="stylesheet" type="text/css">`<br>if you copied the style into the folder.

3. Include a ticker in your HTML. Examples are included in the [demo page](http://zoomten.github.io/cloneticker/demo.html). **You can only have 1 ticker for each mode! (1 horizontal and/or 1 vertical)**

4. Ticker data is split into categories and content.<br> The categories are defined in `cloneTicker-categories.js`.<br><br>The ticker data is dependent on the loaded script within the cloneTicker `div`. In the demo's case, it's `latest.js` and `latest2.js`, loaded with `<script src="tickers/latest.js">`, and `<script src="tickers/latest2.js">` respectively.<br><br>To write different ticker content, you can either edit `testticker_0.js`, or make different files based on it, provided that you change the HTML code accordingly.

License
-
This project is licensed under the [MIT License](LICENSE).