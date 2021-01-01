# 機器學習通識_期末報告

# 組員

陳佑宏, 嚴毅澤, 黃昱東, 林昱辰

# 目標

辨識101種食物，資料集共101000張圖片  
每種食物有1000張圖片，其中800張作為training資料、100張做為validation資料、100張作為testing資料

# 成果

跑了2個epoch，loss還在下降，但由於時間有限沒有繼續跑更多epoch、甚至fine tuning  
最後成果是56% accuracy (隨便猜的話accuracy是1%)

# 準備方式

使用inception_v3做transfer learning  
資料集來源：https://www.kaggle.com/kmader/food41

main.ipynb參考：
1. https://www.itread01.com/content/1549244008.html
2. https://keras.io/api/applications/
3. 其他註解在main.ipynb中

其他程式參考：  
keras、tensorflow官方文件、stackoverflow問答

# 說明

1. main.ipynb： training，輸出model.h5(包括整個模型和其訓練完的權重)
2. inception layers.txt： 解凍inception_v3時察看層數
3. Moving_img_to_train_test_val.ipynb： Split all images into train(80%), validation(10%), test(10%) folders.
4. make_prediction.ipynb： 對test dataset做預測，讀取model.h5、輸出預測結果、輸出confusion matrix圖、輸出accuracy
