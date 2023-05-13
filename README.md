# SP-500-ETF-200MA-Trading-Strategy
#### 作者: Eric Hsu         
#### Date: 2023/05/14


以下為2000年1月至2023年5月S&P 500 ETF價格走勢
![image](https://github.com/EricHsu10/SP-500-ETF-200MA-Trading-Strategy/assets/111495932/6aefee9c-0b09-4b01-8e29-0fdfc93a2ed6)


#### 交易策略
從2000年1月1日開始實做一個簡單的，進出場條件如下:
進場條件:
月底時，SPY的收盤價高於n天的移動平均，在下一個交易日以開盤價買入
出場條件:
月底時，SPY的收盤價低於n天的移動平均，在下一個交易日以開盤價賣出


#### 策略結論
雖然200MA進出場和Buy and Hold最終績效相差不大，但使用MA進出場策略可以有效避開大盤下跌階段，帳面損益較佳，此外若空手階段可以將資金投入其他標的中，達成更好的複利效果。

#### 策略持倉視覺化
其中，股價標示紅色線部分，代表正在持有這檔ETF，Trading Sign為產生進出場訊號，1代表進場，0代表空手。
![image](https://github.com/EricHsu10/SP-500-ETF-200MA-Trading-Strategy/assets/111495932/506f529b-1d6a-4878-82af-c5ae5a51a503)

#### 比較Buy and Hold持有這一檔ETF績效
![image](https://github.com/EricHsu10/SP-500-ETF-200MA-Trading-Strategy/assets/111495932/1e5c3ca3-6f30-4e58-9d3f-9468b2de1f89)

#### 畫每年年化報酬柱狀圖比較
![image](https://github.com/EricHsu10/SP-500-ETF-200MA-Trading-Strategy/assets/111495932/2e2362c2-953f-4aec-8507-702f49e217e0)

#### 策略績效&Drawdown
![image](https://github.com/EricHsu10/SP-500-ETF-200MA-Trading-Strategy/assets/111495932/4a4962cd-30c7-4584-87f7-7604a4f7dcf8)

#### TO DO List
1. 引入更多的指標：嘗試加入更多的技術指標，如RSI，MACD等，來增加進出場的條件，以提高策略的表現。

2. 優化參數：嘗試修改現有指標的參數，例如200MA改成其他的天數，可能可以進行優化，但須考慮是否會發生overfitting問題。

3. 使用機器學習：嘗試使用機器學習方法來預測市場的變動，並根據預測結果來制定交易策略，但也須考慮overfitting問題。

4. 組合策略：可以嘗試將多個策略組合在一起，ex. Long Short S&P and Nasdaq，這可能有助於提高策略的績效並降低風險。
