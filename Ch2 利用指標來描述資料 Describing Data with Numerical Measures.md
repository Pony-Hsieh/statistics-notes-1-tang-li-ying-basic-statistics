# 筆記
## 一、如何以數值指標來描述資料
- 連續型資料有以下特性：
  - 要從圖形中觀察哪些趨勢
  1. 集中趨勢 ("Central Tendency" or "Location")
     - 資料有往資料的中央位置靠近的趨勢
     - 常用的集中趨勢指標
       - 表示一組數據的中央點位置，所在的指標
       - 指標選用
         - mean 對於離群值(outlier)很敏感， median, mode 則否  
           所以資料中有離群值時，建議選用 median, mode；
       1. 平均數 (mean)
        ![](<images/Ch2 利用指標來描述資料 Describing Data with Numerical Measures/2024-06-26 (Wed) 10-16-21.png>)
       2. 中位數 (median)
        ![](<images/Ch2 利用指標來描述資料 Describing Data with Numerical Measures/2024-06-26 (Wed) 13-28-51.png>)
       3. 眾數 (mode)
          - 在一組數據中，出現次數最多的數值；一組數據可以有多個眾數
  2. 分散或變異趨勢 ("Dispersion" or "Variabiblity")
     - 表示一組數據 差異大小 或 數值變化
     - 常用來量測分散趨勢的指標
       1. 全距 (Range, R)
          - 衡量一組數據分散程度，最簡單的方法
          - 算法： 最大值 - 最小值
          - 缺點： 當一組數據中，有出現離群值，或者資料筆數太多時(n > 10)，全距並非一個很好的指標來衡量分散程度，因為他沒辦法看出最大值、最小值之間數據分佈的狀況
          - ![](<images/Ch2 利用指標來描述資料 Describing Data with Numerical Measures/2024-06-26 (Wed) 15-40-06.png>)
       2. 變異數 (Variance)
        ![](<images/Ch2 利用指標來描述資料 Describing Data with Numerical Measures/2024-06-26 (Wed) 15-46-01.png>)
          - 分母一定要除 [數據總數 - 1]
            - 一種簡單的理解方式是，平方之後，數值的分佈會與原始狀況有差異，因此透過調整分母來微調
          - 取平方是為了避免正負相消
          - 假設一組數據中，所有的值都相同，則變異數為 0，標準差也為 0
          - 標準差和變異數，是衡量一組數據絕對變異(absolute variation)的指標，也就是這個指標的大小，和單位有關；因此，如果需要一個指標來比較不同單位的數據時，可以選用變異係數
       3. 標準差 (Standart Deviation, SD)
          - 變異數開根號
          - 實務上比較常用這個，因為變異數的話，單位會帶平方
          - 用全距來估計標準差
            ![](<images/Ch2 利用指標來描述資料 Describing Data with Numerical Measures/2024-06-26 (Wed) 16-57-51.png>)
       4. 變異係數 (Coefficient of Variation, CV)
          - 綜合考量標準差和平均數的指標，用來衡量資料的相對分散程度，是一個沒有單位的指標
          ![](<images/Ch2 利用指標來描述資料 Describing Data with Numerical Measures/2024-06-26 (Wed) 17-52-59.png>)
  3. 偏態 (Skewness)
     - 一組數據分佈的型態(shape of a distribution)
       ![](<images/Ch2 利用指標來描述資料 Describing Data with Numerical Measures/2024-06-26 (Wed) 18-02-27.png>)
       ![](<images/Ch2 利用指標來描述資料 Describing Data with Numerical Measures/2024-06-26 (Wed) 18-04-22.png>)
       ![](<images/Ch2 利用指標來描述資料 Describing Data with Numerical Measures/2024-06-26 (Wed) 18-04-36.png>)
  4. 峰度 (Kurtosis)
- 當你手邊有一大堆數據的時候，你根本沒有辦法理解這些數據所代表的含意；透過指標，你可以從不同的角度去理解這些數值的樣貌、特性
- 數據量夠大的時候，就可以把樣本 "視作" 群體；不然通常其他狀況下，都是拿樣本去 "推論" 群體


# 影片
- [Lec02 統計學(一)(基礎統計) Ch2 利用指標來描述資料 Describing Data with Numerical Measures](https://www.youtube.com/watch?v=GP_Fi8t0UwI&list=PLj6E8qlqmkFvsst4-ww1mrax1D65FQI1m&index=2)