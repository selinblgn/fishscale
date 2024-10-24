
Fish Dataset Üzerinde Yapay Sinir Ağı (ANN) ile Sınıflandırma

Proje Hakkında

Bu proje, Kaggle'dan alınan Large-Scale Fish Dataset üzerinde bir Yapay Sinir Ağı (Artificial Neural Network - ANN) modeli kullanarak balık türlerini sınıflandırmayı amaçlamaktadır. Projede, veri setindeki görüntüler üzerinde bir derin öğrenme modeli eğitilmiştir. Modelin performansı eğitim ve doğrulama setlerinde takip edilmiştir.

Veri Seti

Kullanılan veri seti Kaggle üzerinde bulunan Large-Scale Fish Dataset'tir. Bu veri seti, çeşitli balık türlerinin görüntülerini içermektedir ve balık sınıflandırma görevinde kullanılmıştır. Veri setine buradan (https://www.kaggle.com/datasets/crowww/a-large-scale-fish-dataset) ulaşabilirsiniz.

Veri Seti Yapısı

Her görüntü, bir balık türünü temsil eder ve görüntüler farklı boyutlardadır. Proje boyunca, tüm görüntüler modele uygun hale getirmek için 64x64 piksel boyutuna yeniden boyutlandırılmıştır.

Model Yapısı

Bu projede, temel bir Yapay Sinir Ağı (ANN) modeli kullanılmıştır. Model, balık görüntülerini sınıflandırmak için eğitilmiştir.
Giriş Katmanı: 64x64 boyutundaki (3 kanallı RGB) görüntüler için Flatten katmanı.
Gizli Katmanlar: İki gizli katman kullanılmıştır. İlk katman 128 nörona, ikinci katman ise 64 nörona sahiptir ve her ikisi de ReLU (Rectified Linear Unit) aktivasyon fonksiyonunu kullanır.
Çıkış Katmanı: Son katman, balık türlerini temsil eden sınıf sayısı kadar nörona sahiptir ve Softmax aktivasyon fonksiyonunu kullanarak sınıflandırma yapar.
Model, eğitim veri seti üzerinde eğitilmiş ve doğrulama veri seti ile test edilmiştir. Eğitim ve doğrulama doğruluğu grafiklerle takip edilmiştir. Eğitim süreci boyunca 100 epoch boyunca model eğitilmiştir.

Sonuçlar

Eğitim Doğruluğu: %100'e yakın bir eğitim doğruluğu elde edilmiştir.
Doğrulama Doğruluğu: Son epoch'ta doğrulama doğruluğu %98.64 olarak ölçülmüştür.
Bu sonuçlar, modelin balık türlerini oldukça başarılı bir şekilde sınıflandırdığını göstermektedir. 
Bu değerler, modelin eğitim verisine çok iyi uyduğunu ve doğrulama verisinde de oldukça başarılı olduğunu göstermektedir.

Adresler
-Kaggle Notebook:https:https://www.kaggle.com/code/ayeselinbilgin/fishscale/edit

-Kaggle Dataset:https://www.kaggle.com/datasets/crowww/a-large-scale-fish-dataset
