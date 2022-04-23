# populationdensity 人口密度地圖
這個網站簡單扼要的呈現台灣人口密度的高地分布，以分層設色的方式呈現，具體處理步驟如下：
# step 1 圖資整合
利用政府的opendata取得台灣型性區圖的shp，再去各里取得各行政區的人口資料，最後打開GIS用join的方式將兩個資料整合再一起。
# step 2 轉檔 conversion
因為一次將shp轉成geojson，會太大(116 MB)所以這邊會建議是分縣市去個別轉成geojson，
最後再將.geojson以檔名的方式改成.js
# step 3 Coding 
打開VS把建立一個檔案，以leaflet為基礎，設定對話框、互動、zoom等等細節都在index裡面，就可以了。
