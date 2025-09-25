### Cezayir Orman Yangınları Veri Analizi ve Makine Öğrenmesi Modeli

Bu proje, Cezayir orman yangınlarına ait verileri analiz ederek yangın riskini tahmin etmeyi amaçlayan kapsamlı bir veri temizleme, keşifçi veri analizi (EDA) ve makine öğrenmesi çalışmasını içermektedir.

### Kullanılan Araçlar ve Kütüphaneler

Projede kullanılan Python kütüphaneleri şunlardır:

* **pandas**: Veri işleme ve analizi için temel kütüphane.
* **numpy**: Sayısal işlemler ve dizilerle çalışmak için.
* **matplotlib.pyplot**: Veri görselleştirme için.
* **seaborn**: İstatistiksel grafikler oluşturmak için.
* **sklearn**: Makine öğrenmesi modeli oluşturmak ve değerlendirmek için.

### Veri Seti

Bu proje, Kaggle üzerinden sağlanan `Algerian_forest_fires_dataset.csv` veri setini kullanmaktadır. Veri seti, 2012 yılına ait sıcaklık, nem, rüzgar hızı ve yağış gibi çeşitli iklim ve hava durumu metriklerini içerir. Hedef değişken (`Classes`), orman yangını olup olmadığını (`fire` veya `not fire`) belirtmektedir.

### Analiz ve Modelleme Adımları

Projede izlenen temel adımlar şunlardır:

1.  **Veri Temizleme**: Veri setindeki eksik ve yanlış girilmiş değerler tespit edilip temizlenmiştir. Kolon adlarındaki gereksiz boşluklar kaldırılmış ve veri tipleri uygun formatlara dönüştürülmüştür.
2.  **Keşifçi Veri Analizi (EDA)**: Kategorik ve sayısal veriler arasındaki ilişkiler ve dağılımlar görselleştirilerek incelenmiştir.
3.  **Makine Öğrenmesi Modeli**:
    * Veri seti, eğitim ve test setleri(Train Test Split) olarak ayrılmıştır.
    * **ElasticNetCV** modeli kullanılarak bir yangın tahmini modeli oluşturulmuştur.
    * Modelin performansı, **Ortalama Mutlak Hata (MAE)**, **Ortalama Karesel Hata (MSE)** ve **R2 Skoru** metrikleri kullanılarak değerlendirilmiştir.

### Nasıl Çalıştırılır?

Bu projeyi kendi bilgisayarınızda çalıştırmak için şu adımları takip edebilirsiniz:

1.  Gerekli kütüphaneleri yükleyin:
    `pip install pandas numpy matplotlib seaborn plotly scikit-learn`
2.  `algeria-forest-fires.ipynb` dosyasını Jupyter Notebook'ta açın ve hücreleri sırayla çalıştırınız.

### Kaggle Proje Linki: https://www.kaggle.com/code/mehmetren/algeria-forest-fires
