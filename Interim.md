
# 蒙地卡羅法
* 聲明: 內容複製自參考資料文章,加上部分註解&心得
> 
# 引言:
* 蒙地卡羅方法（英語：Monte Carlo method），也稱統計類比方法，
 是1940年代中期由於科學技術的發展和電腦的發明，而提出的一種以機率統計理論為指導的數值計算方法。是指使用亂數（或更常見的偽亂數）來解決很多計算問題的方法。

# 應用領域：
* 金融
* 項目管理
* 能量
* 製造業
* 工程學
* 研究和開發
* 保險
* 石油和天然氣公司
* 交通
* 環境

# 舉例:

## 拋硬幣示例

* 拋硬幣中獎的概率是1/2。在這個例子中，我們將使用蒙特卡羅方法迭代地模擬拋硬幣5000次，以找出為什麼頭部或尾巴的概率總是1/2。如果我們重複拋硬幣很多很多次，
那麼我們可以在概率值的準確答案上獲得更高的精確度。在這個例子中，我們將使用Monte-Carlo方法反覆模擬拋硬幣5000次，以找出頭部或尾部的概率始終是1/2的概率。
在這個例子中，我們將使用蒙特卡羅方法迭代地模擬拋硬幣5000次，以找出為什麼頭部或尾巴的概率總是1/2。如果我們重複拋硬幣很多很多次，那麼我們可以在概率值的準確答案上獲得更高的精確度。
在這個例子中，我們將使用Monte-Carlo方法反覆模擬拋硬幣5000次，以找出頭部或尾部的概率始終是1/2的概率。

> 1.導入所需的庫：  //正面和反面，數學表示。
>
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f6874cd408b1.png?imageView2/2/w/740 "正面與反面")

> 2.投幣功能：  //一個簡單的函數，將結果隨機排列在0和1之間，頭部為0，尾部為1。
> 
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f6875412f442.png?imageView2/2/w/740 "投硬幣功能")

> 3.檢查函數輸出：  //運行Coin_Flip()函數
> 
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687561a527d.png?imageView2/2/w/740 "檢查函數輸出")

> 4.主要功能：  //計算概率並將概率值附加到結果。
> 
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f6875827eb8a.png?imageView2/2/w/7400 "主要功能")

> 5.調用main函數：  //調用Monte Carlo主函數，並繪製最終值。
> 
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f6875a3172df.png?imageView2/2/w/740 "調用main函數")



## 為什麼賭場總是賺的？
* 賭場是怎麼賺錢的？ 訣竅很簡單–「你玩得越多，他們賺的就越多。」 讓我們通過一個簡單的蒙特卡羅模擬示例來看看這是如何工作的。

* 考慮一個假想的遊戲，玩家必須從一袋籌碼中選擇一個籌碼。

* 規則：
  * 袋子里有數字從1到100的籌碼。
  * 用戶可以押注於偶數或奇數籌碼。
  * 在這個遊戲中，10和11是特殊的數字。 如果我們賭偶數，那麼10就算奇數，如果我們賭賠率，那麼11就算偶數。
  * 如果我們賭偶數，我們得了10，那麼我們就輸了。
  * 如果我們賭的是奇數，我們得了11，那麼我們就輸了。
 * 如果我們以賠率下注，我們獲勝的概率為49/100。 獲勝的概率為51/100。 因此，對於一個奇數下注，彩池優勢為= 51 / 100–49 / 100 = 200/10000 = 0.02 = 2％
 * 如果我們打賭偶數，則用戶獲勝的概率為49/100。 獲勝的概率為51/100。 因此，對於一個奇數下注，彩池優勢為= 51 / 100–49 / 100 = 200/10000 = 0.02 = 2％
 * 綜上所述，每下注1美元，就會有0.02美元下注。 相比之下，輪盤上最低的單一0優勢是2.5％。 因此，我們可以肯定，與輪盤賭相比，您在假想的遊戲中獲勝的機會更大。
 
> 1.Import所需的庫:  // 導入賭場模擬所需的庫。
>
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687a5ae02ff.png?imageView2/2/w/740 "正面與反面")

> 2. 玩家下注:  // 在下注奇數或偶數。
>
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687a663368e.png?imageView2/2/w/740 "正面與反面")

> 3. Main 函數:  // 使用蒙特卡洛方法模擬賭場行為。
>
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687a663368e.png?imageView2/2/w/740 "正面與反面")

> 4. 最終輸出: // 計算並展示計算結果。
>
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687a852f921.png?imageView2/2/w/740 "正面與反面")

> 5. 模擬1000次試試: // 模擬1000次。
>
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687a92c9cc0.png?imageView2/2/w/740 "正面與反面")

> 6. 下注數 = 5: // 下注5次時的結果可視化。
>
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687af2c64f9.png?imageView2/2/w/740 "正面與反面")

> 7.  下注數 = 10: // 下注10次時的結果可視化。
>
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687afed37a3.png?imageView2/2/w/740 "正面與反面")

> 8.  下注數 = 1000: // 下注1000次時的結果可視化。
>
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687b0a9d419.png?imageView2/2/w/740 "正面與反面")

> 9.  下注數 = 5000: // 下注5000次時的結果可視化。
> 
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687b157f1d6.png?imageView2/2/w/740 "正面與反面")

> 10.  下注數 = 10000: // 下注10000次時的結果可視化。
> 
![GITHUB]( https://static.leiphone.com/uploads/new/images/20200921/5f687b2208454.png?imageView2/2/w/7400 "正面與反面")

* 從上面的實驗中，我們可以看到，如果玩家在賭博中下注較少，那麼有得賺的機會就比較大。有時候實驗會得到負數，這意味著玩家輸得傾家蕩產負債纍纍，而不是單車變路虎。
        
* 結論:
  * 就像任何預測模型一樣，模擬結果只有估計值才是好的，但蒙特卡洛模擬只代表概率而不是確定性。儘管如此，在預測未知的未來時，蒙特卡洛模擬是一個有價值的工具。

 
 
 
### 參考資料:
https://zh.wikipedia.org/wiki/%E8%92%99%E5%9C%B0%E5%8D%A1%E7%BE%85%E6%96%B9%E6%B3%95

https://codingnote.cc/zh-tw/p/210692/




