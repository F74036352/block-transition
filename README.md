# block-transition
各頁面介紹:
1.	Index.html:遊戲開始的進入畫面。

2.	story.html:故事背景介紹以及遊戲說明。

3.	game.html:開始石板傳送的遊戲，此版本為一開始的原始版本，玩家會因為缺少許多傳送時需要的資訊，導致時常發生傳送錯誤或是遺失的情形。

4.	introduction.html:解釋game.html中的模式為何會發生失敗，並給予玩家提示及反思，引領玩家進入下一個修改過的模式。

5.	gameFixed.html:與game.html的規則相同，但加入了某些確保傳送過程是正確的機制，提升傳送的正確率。

6.	final.html:介紹網路通訊的封包傳送，解釋此遊戲所欲帶給玩家的知識以及遊戲中各項機制所代表的意義。







使用技術:
CSS: 
1.	font-siz->調整字體大小。
2.	text-align: center->排版置中。
3.	background: url(#)->設定圖片及背景。
4.	color->更改字體顏色。
5.	font: Tahoma bold->更改字型設為粗體。
6.	text-shadow: 0.5px 0.5px 0.5px black->設定字體的陰影及陰影顏色為黑色。

html5:
1.	<p>:設定文字。
2.	<img>:設定圖片。
3.	<a href=”#”>:設定連結。
4.	<button onclick="#">:設定按鈕以及按下去後所執行的動作。
5.	<input type="text" id="myText" maxlength="2">:設定輸入文字的欄位以及限制輸入的長度。




Javascript:
1.	function scrollwindow():使用window.scrollTo使頁面達到自動下拉的效果。
2.	function startit():藉由setInterval("scrollwindow()",35)設定多久會下拉一次，而一次下拉多少在scrollwindow()中有設定。
3.	function getQusetion():
將所有可能先宣告-> var possible = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789";
再使用亂數產生長度，產生石板傳送時的題目。
4.	function sendMode():依照遊戲規定從三種mode中，隨機選擇一種石板傳送的mode。
5.	function sendText():依照產生的mode，選擇傳送的過程會發生的事情以及最後的結果。
6.	function sent(text):顯示收到的石板訊息。
7.	function gameEnd():最後遊戲結束時顯示的訊息。
