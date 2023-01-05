# Deep-Learning-Final
Efficient deep learning approach for augmented detection of Coronavirus disease

**Referans Paper** <br/>
[Efficient deep learning approach for augmented detection of Coronavirus disease](https://doi.org/10.1007/s00521-020-05410-8)

Çalışmada 4 adet veriseti kullanılmış fakat 2. veriseti ikiye bölünerek toplam 5 veriseti elde edilmiştir. Bu veri setlerini eğitmek için ise 2 adet model oluşturulmuştur. Bunlar; CNN ve Hibrit CovnLSTM modelleridir.

**VERİSETLERİ**

**Veriseti 1** [COVID-CT-Dataset (2020) A CT scan dataset about COVID-19.](https://github.com/UCSD-AI4H/COVID-CT.)

**Veriseti 2** [Alqudah AM, Qazan S (2020) Augmented COVID-19 x-ray images dataset](https://doi.org/10.17632/2FXZ4PX6D8.4)

**Veriseti 3** [Accessed 15 Oct 2020](https://www.kaggle.com/tawsifurrahman/covid19-radiographydatabase.)

**Veriseti 4** [Sedik A, El-Samie A, Fathi E, El-Latif A, Ahmed A, Hammad M (2020) Combined COVID-19 dataset.](https://doi.org/10.17632/3pxjb8knp7.3)

![Verisetleri](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/Tablolar/veriseti.PNG)

**MODELLER**

**1.CNN Modeli** <br/>

![CNN Model kod](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/MODELLER/CNN%20MODEL.PNG)
![CNN Model Çıktı](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/MODELLER/CNN.png)

**2. Hibrit CovnLSTM Modeli** <br/>

![CovnLSTM Model kod](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/MODELLER/CovnLSTM%20MODEL.PNG)
![CovnLSTM Model Çıktı](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/MODELLER/CovnLSTM.png)

**SONUÇLAR** <br/>
Veriseti ve model kombinasyon sonuçları, ayrı ayrı klasörlerde Result klasörü içerisinde bulunmaktadır. <br/>
Aşağıda genel olarak 1. Model olan CNN Modeli için scorelar tablolaştırılmıştır.

![Sonuç Tablo](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/Tablolar/CNN%20Score.PNG)



