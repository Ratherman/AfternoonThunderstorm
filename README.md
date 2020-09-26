# 臺北午後雷陣雨預報系統

## 於雲端環境執行本專案:
1. 請參考下方 google colab 連結以獲得更完整內容
https://colab.research.google.com/drive/1f4IxFYRUHYMVYePqBbJq8pXyw6ZueoxK?authuser=0#scrollTo=Ru4-q4VuUSbO
2. 或是直接下載 Copy_of_臺北午後雷陣雨預報系統.ipynb 並且用 google colab 打開。
3. 不需要特別安裝什麼套件

## 於本地端執行本專案需要以下套件
1. jupyter notebook
2. scikit learn
3. pandas

# 針對爬取 氣象局 觀測資料查訊系統 請直接在 third_party 資料夾內 clone 此下方專案
專案連結:https://github.com/s3131212/CWB-Observation-Crawler

# 步驟說明
1. 爬取資料: 
* 利用 third_party/ 的 UWYO-SoundingData-Crawler，能夠取得板橋測站的 sounding data
* 利用此專案連結(https://github.com/s3131212/CWB-Observation-Crawler ) 可以爬取地面測站資料。

2. 合併資料:
* 使用 src/ 內的 Combine_Data.ipynb (Jupyter Notebook)合併探空資料和地面測站資料

3. 機器學習
* 使用 src/ 內的 model.ipynb 可以簡單的做到機器學習。