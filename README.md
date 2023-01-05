# Derin-Öğrenme-Final
**Coronavirüs hastalığının artırılmış tespiti için verimli derin öğrenme yaklaşımı** <br/>
COVID-19, hızla güncelliğini yitiren istatistiklerle dünya nüfusunu hızla etkilemektedir. Açıklamalı Coronavirüs Röntgen ve BT görüntülerinin sınırlı mevcudiyeti nedeniyle, COVID-19'un saptanması, bu hastalığın teşhisinde en büyük zorluk olmaya devam etmektedir. Çalışmada, önerilen derin öğrenme yöntemleri, evrişimli sinir ağı (CNN) ve evrişimli uzun kısa süreli belleğe (ConvLSTM) dayanmaktadır. <br/>
Önerilen modellerin simülasyonu için iki farklı veri seti benimsenmiştir. İlk veri seti bir dizi CT görüntüsü içerirken, ikinci veri seti bir dizi X-ışını görüntüsü içerir. Bu veri kümelerinin her ikisi de iki kategoriden oluşur: COVID-19 ve normal. Ek olarak, önerilen modelleri doğrulamak için (3.veri seti) COVID-19 ve pnömoni görüntü kategorileri sınıflandırılmıştır. Önerilen derin öğrenme modelleri, hem X-ışını hem de CT görüntüleri ile her iki görüntü türünü içeren birleşik bir veri kümesi olan 4. veriseti üzerinde test edilir.


**Referans Çalışma** <br/>
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

![CNN Model kod](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/MODELLER/CNN%20MODEL%C4%B0.PNG) <br/>
![CNN Model Çıktı](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/MODELLER/CNN.png)

**2. Hibrit CovnLSTM Modeli** <br/>

![CovnLSTM Model kod](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/MODELLER/CovnLSTM%20MODEL.PNG) <br/>
![CovnLSTM Model Çıktı](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/MODELLER/CovnLSTM.png)

**SONUÇLAR** <br/>
Veriseti ve model kombinasyon sonuçları, ayrı ayrı klasörlerde Result klasörü içerisinde bulunmaktadır. <br/>
Aşağıda genel olarak 1. Model olan CNN Modeli için scorelar tablolaştırılmıştır.

![Sonuç Tablo](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/Tablolar/CNN%20Score.PNG)

**Accuracy ve Loss Grafikleri** <br/>
CNN Modeli sırasıyla 1, 2-A, 2-B, 3 ve 4. veriseti üzerinde ayrı ayrı çalıştırılmıştır. Her eğitim için train verisetinden veriler %70 train ve %30 validation veri olarak ayrılmıştır. Epoch 40, batch size olarak referansa sadık kalınmaya çalışılmış 20 kullanılmış fakat verisetine göre 32 ve 256 da kullanılmıştır. <br/>
Aşağıda sırasıyla verisetlerinin, train ve val değerlerinin 40 epoch üzerinde accuracy ve loss sonuçlarının grafikleri çizdirilmiştir.

![veriseti 1](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/1%20CNN/acc%20loss.png)
![veriseti 2a](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/2%20%20A%20CNN/acc%20loss.png)
![veriseti 2b](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/2%20B%20CNN/acc%20loss.png)
![veriseti 3](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/3%20CNN/acc%20loss.png)
![veriseti 4](https://github.com/merveenbiya/Deep-Learning-Final/blob/main/Results/4%20CNN/ACC%20LOSS.png)

