# 筆記
## 一、甚麼是二元變數資料？
- 在進行研究調查時，經常需要蒐集、分析多個變數的資料，以探討變數間的關聯性  
例如：
  1. 某經濟系教授想要知道一個大學生每週花在餐飲的金額與該生家庭年收入間的關聯性
  2. 某房屋仲介商想知道房價與房子坪數間的關聯性
  3. 某工程師想知道晶圓良率與晶圓缺陷點數的關聯性
## 二、常見二元 類別 變數圖型
### side-by-side bar chart
- 將兩類別 **並列** 在一起之長條圖
 ![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-12 (Wed) 17-00-14.png>)
### stacked bar chart  
- 將兩類別 **堆疊** 在一起之長條圖
  ![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-12 (Wed) 17-00-54.png>)
- 這還多視覺化了兩類別總計的資料
### side-by-side pie chart  
- 將兩類別 **並列** 在一起之圓餅圖
  ![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-12 (Wed) 17-04-12.png>)
## 三、常見二元 數值 變數圖型
### 二維散佈圖 (x-y scatter plot(diagram))
- 限制：
  - 只能用在連續型資料、數值資料，類別型資料就比較不適用
- 觀察重點
  1. 你觀察到甚麼圖型？  
    直線？ 曲線？ 隨機分佈？
  2. 圖案是否明顯？
  3. 圖型中是否有離群值(outlier)？
- 範例
  ![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-12 (Wed) 17-10-40.png>)
  ![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-12 (Wed) 17-11-21.png>)
## 四、二元數值變數之量化指標
![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-28 (Fri) 10-45-02.png>)
### 共變異數 (Covariance, Cov)
![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-28 (Fri) 10-45-48.png>)
- 如果只有一組資料，變異數長這樣：  
  ![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-28 (Fri) 10-47-18.png>)
  - 共變異數，就只是把(x - μₓ)²，換成 (x - μₓ)(y - μᵧ)
- Cov 是有單位的
### 相關係數 (Correlation Coefficient)
- 算法： 兩變數的共變異數除以各變數之標準差的乘積
![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-28 (Fri) 10-51-54.png>)
- 相關係數沒有單位
- 相關係數必然介於正負 1 之間
- 數值解讀：
  - |r| 越接近 1，只能說明這兩者的線性關係越強；  
    |r| 越接近 0，只能說明這兩者越沒有線性關係(不一定沒有關係，有可能是其他關係，例如曲線關係)
  - |r| ≥ 0.8，代表有夠強的線性關係
## 五、x-y 之直線方程式 = 迴歸方程式 = 最小平方線
![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-28 (Fri) 11-48-12.png>)
![](<images/Ch3 利用指標來描述雙變量資料 Describing Bivariate Data/2024-06-28 (Fri) 11-48-22.png>)
- 如果 r 很低的話，這條線就不用找了，因為找了也沒有意義
- 斜率 b 代表，x 每增減 1，y 值變化的程度


# 影片
- [Lec03 統計學(一)(基礎統計) Ch3 利用指標來描述雙變量資料 Describing Bivariate Data](https://www.youtube.com/watch?v=HpxQoQYZAvw&list=PLj6E8qlqmkFvsst4-ww1mrax1D65FQI1m&index=3)