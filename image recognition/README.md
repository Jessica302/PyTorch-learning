# Image recognition
將多個特徵經過softmax函數把值映射到0,1之間，輸出10個類別。其中利用自動計算梯度和GPU加速模型計算，建置衣服、包包等圖片預測模型。

### 訓練步驟
1. 使用Pytorch官網提供的FashionMNIST datasets<br>
<img src="https://github.com/Jessica302/PyTorch-learning/blob/main/image%20recognition/image/image.png" width=30%>
2. 將圖片轉成tensor格式<br>
3. 使用dataloader將60000張圖片分batch，比較好進行模型訓練<br>
4. 建立模型，包含攤平和定義正向傳播<br>
5. batch輸入模型進行訓練<br>
6. 計算預測數據跟真實資料的損失函數(CrossEntropy交叉熵)<br>
7. 設定優化器(SGD梯度下降法)，透過最小化損失函數去調整w,b，讓模型預測更接近真實資料<br>
8. 進行多次模型計算，透過更新w,b參數，觀察cost下降過程跟準確率<br>
<img src="https://github.com/Jessica302/PyTorch-learning/blob/main/image%20recognition/image/result.png" width=50%>
