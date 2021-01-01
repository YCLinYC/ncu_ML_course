# 機器學習通識_期末報告

### Due date
2021/1/4

### Team member
陳佑宏, 嚴毅澤, 黃昱東, 林昱辰

# 準備方式

使用keras.applications.inception_v3
參考：
1. https://www.itread01.com/content/1549244008.html
2. https://keras.io/api/applications/
3. 其他註解在main.ipynb中

# 說明

1. main.ipynb： 主程式
2. inception layers.txt： 查看inception_v3層數
3. grab_plots_from_here.ipynb： 翻出來的舊程式，讀資料方式會占用大量RAM，可以copy繪圖
4. Moving_img_to_train_test_val.ipynb： Split all images into train(80%), validation(10%), test(10%) folders.
5. make_prediction.ipynb： 對test dataset做預測讀取model.h5、輸出預測結果、輸出confusion matrix圖、輸出accuracy
