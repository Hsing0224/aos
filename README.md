# aos
accordion by jquery<br><a href="https://starrandy.github.io/aos/">您也可以在這邊看</a>
## 功能
  1. [用法](#用法)
  2. [模式](#模式)
  3. [持續時間](#持續時間)
  4. [動畫](#動畫)
  5. [指定開啟](#指定開啟)
  6. [導引宣告](#導引宣告)
  7. [自動加入高度](#自動加入高度)
  8. [以導引為按鈕](#以導引為按鈕)
  9. [上一步](#上一步)
  10. [下一步](#下一步)
  11. [進行中](#進行中)
  12. [麵包屑](#麵包屑)

##	用法
載入<a href="http://jquery.com/download/">jQuery主程式</a>，並將aos.js放在&lt;head&gt;或&lt;/body&gt;前<br>
使用.aos，結構必須為以下範例(標籤依開發者自己調整)
```html
	<ul class="aos"> <!-- 以下的相關設定可在此加入 -->
	  <li> <!-- 需把標題和內容包起來 -->
	    <h6>標題</h6>
	    <div>內容</div>
	  </li>
	  <li>
	    <h6>標題</h6>
	    <div>內容</div>
	  </li>
	</ul>
```
##	模式
預設為.aos的第一層子元素才有效果，如需設定為選單模式，可在.aos加入屬性data-mode="menu"

##	持續時間
開收合效果的動畫時間，預設為300，也可自定義在.aos加入屬性data-duration="持續時間(ms)"

##	動畫
開收合的動畫效果，預設為linear，<br>可下載類似<a href="http://easings.net/zh-tw" target="_blank">Easing 函數速查表</a>等擴充動畫效果，<br>利用.aos加入屬性data-easing="函數名稱"

##	指定開啟
當頁面載入，如需先將某項內容開啟，可在內容的標籤裡加上屬性data-open，<br>注意的是當載入好頁面，data-open是會被自動移除的
```html
	<ul class="aos">
	  <li>
	    <h6>標題</h6>
	    <div data-open>內容</div> <!-- 將data-open加入此項目 -->
	  </li>
	  <li>
	    <h6>標題</h6>
	    <div>內容</div>
	  </li>
	</ul>
```

##	導引宣告
可在.aos裡加入data-guide="自定義類別"，會自動在需開啟的標題加入導引的按鈕，<br>當開啟狀態時，data-guide會加上.open<br>
note:當未啟用data-guide，可以利用.aos-active、.aos-bread來達成.open

##	自動加入高度
如有在.aos加入data-guide，可利用data-guide-height，將標題的高度帶入data-guide

##	以導引為按鈕開啟
如需只有當按下data-guide時才開啟內容，可在.aos加入data-guide-btn

##	上一步
如在按鈕加上.aos-prev，按下則可以自動收合並開啟上一個內容

##	下一步
如在按鈕加上.aos-next，按下則可以自動收合並開啟下一個內容

##	進行中
當前所開啟的項目，該選項會自動加入.aos-active

##	麵包屑
凡走過必留下痕跡，當有階層性時，會自動加入.aos-bread
