README.md
🏠 Konut Fiyatı Tahmin Projesi
Bu proje, konut özelliklerini kullanarak makine öğrenmesi regresyon algoritmaları ile konut fiyatlarını tahmin etmeyi amaçlamaktadır.
Proje kapsamında veri analizi, veri ön işleme, özellik dönüşümü, farklı regresyon modellerinin eğitilmesi ve model performanslarının karşılaştırılması gerçekleştirilmiştir.
🎯 Projenin Amacı
Konut verileri üzerinden fiyat tahmini yapabilen makine öğrenmesi modelleri geliştirmek ve farklı regresyon algoritmalarının performanslarını karşılaştırmak.
🛠️ Kullanılan Teknolojiler
* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Matplotlib
* Seaborn
* Jupyter Notebook

📊 Proje Aşamaları
1. Keşifsel Veri Analizi (EDA)
Veri setinin yapısını ve değişkenler arasındaki ilişkileri incelemek amacıyla:
* Veri setinin genel yapısı incelendi.
* Sayısal ve kategorik değişkenler analiz edildi.
* Eksik değerler kontrol edildi.
* Değişkenlerin dağılımları incelendi.
* Veri ilişkileri görselleştirildi.
2. Veri Ön İşleme
Modelleme öncesinde veri setine aşağıdaki işlemler uygulandı:
* Eksik veriler SimpleImputer ile ele alındı.
* Sayısal değişkenler StandardScaler ile ölçeklendirildi.
* Kategorik değişkenler OneHotEncoder ile sayısal forma dönüştürüldü.
* Farklı veri tipleri için uygulanacak işlemler ColumnTransformer kullanılarak yapılandırıldı.
* Veri ön işleme ve modelleme adımları Pipeline kullanılarak birleştirildi.
* Veri, eğitim ve test kümelerine ayrıldı.

🤖 Kullanılan Modeller
Projede dört farklı regresyon algoritması kullanılmıştır:
1. Linear Regression
2. Random Forest Regressor
3. Gradient Boosting Regressor
4. XGBoost Regressor
Modeller aynı veri ön işleme sürecinden geçirilerek eğitilmiş ve test veri seti üzerinde değerlendirilmiştir.

📏 Değerlendirme Metrikleri
Model performanslarını değerlendirmek için aşağıdaki metrikler kullanılmıştır:
MAE — Mean Absolute Error
Tahminlerin gerçek değerlerden ortalama mutlak sapmasını ölçer. Daha düşük değer daha düşük ortalama tahmin hatasına işaret eder.
RMSE — Root Mean Squared Error
Tahmin hatalarının karelerinin ortalamasının karekökünü ifade eder. Büyük hatalara MAE'ye göre daha fazla ağırlık verir.
R² — R-Squared
Modelin hedef değişkendeki varyansı ne ölçüde açıkladığını gösterir. Değerin 1'e yaklaşması daha yüksek açıklama gücünü ifade eder.

📈 Model Sonuçları

Modeller test veri seti üzerinde değerlendirilmiştir.

Model            	MAE	          RMSE	      R²

Linear Regression	15,272.67	   21,524.40  	 0.9161

Random Forest	    16,357.63	    23,824.99	   0.8972

Gradient Boosting	 15,429.90	  21,423.99	   0.9169

XGBoost	          16,487.69	    24,037.63	   0.8954

🔎 Sonuçların Değerlendirilmesi
Model sonuçları karşılaştırıldığında:
* Linear Regression modeli 0.9161 R² değerine ulaşmıştır.
* Gradient Boosting modeli 0.9169 ile en yüksek R² değerini elde etmiştir.
* Gradient Boosting modeli aynı zamanda 21,423.99 ile en düşük RMSE değerine sahiptir.
* Random Forest modeli 0.8972 R² değerine ulaşmıştır.
* XGBoost modeli 0.8954 R² değeri elde etmiştir.
Bu sonuçlar, kullanılan veri seti ve uygulanan veri ön işleme adımları kapsamında modellerin performanslarının birbirinden farklı olduğunu göstermektedir.

📁 Proje Yapısı

konut-fiyati-tahmin/
│

├── data/
│   └── housing.csv
│

├── notebooks/
│   └── konut_fiyati_tahmin.ipynb
│

├── README.md

├── requirements.txt

└── .gitignore

⚙️ Kurulum
Repository'yi klonlayın:
git clone https://github.com/USERNAME/konut-fiyati-tahmin.git
cd konut-fiyati-tahmin
Gerekli Python paketlerini yükleyin:
pip install -r requirements.txt
Jupyter Notebook'u başlatın:
jupyter notebook
Ardından:
notebooks/konut_fiyati_tahmin.ipynb
dosyasını açarak projeyi çalıştırabilirsiniz.

📦 Kullanılan Kütüphaneler
* pandas — Veri analizi
* numpy — Sayısal işlemler
* matplotlib — Veri görselleştirme
* seaborn — İleri veri görselleştirme
* scikit-learn — Veri ön işleme, modelleme ve değerlendirme
* xgboost — Gradient boosting tabanlı regresyon
* jupyter — Etkileşimli notebook ortamı

🚀 Gelecekte Yapılabilecek Geliştirmeler
* Hyperparameter tuning uygulanması
* Cross-validation kullanılması
* Feature engineering çalışmalarının geliştirilmesi
* Daha fazla regresyon algoritmasının test edilmesi
* Model sonuçlarının görselleştirilmesi
* Tahmin sonuçlarının gerçek değerlerle karşılaştırılması
* Modelin web uygulaması veya API olarak yayınlanması

👨‍💻 Proje Hakkında
Bu proje, makine öğrenmesi, veri analizi ve regresyon modelleri konularında uygulamalı deneyim kazanmak amacıyla geliştirilmiştir.
