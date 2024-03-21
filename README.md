# Naive Bayes Ödevi
## Intro :
naive bayes modelini diabetes verisi üzerinde kullanarak farklı sonuçları karşılaştırdık

## Method :
python dili ve numpy, sklearn, pandas kütüphaneleri kullanılarak model oluşturulup geliştirilmiştir
hyperparameter tuning için gridsearch, randomsearch kullanılmıştır
feature scaling için PowerTransformer ve QuantileTransformer kullanılmıştır

## Results :
base line model 0.73 accuracy vermiştir, hyperparameter tuning in büyük bir katkısı olmadı
QuantileTransformer ile yapılan normalizasyon işe yarayıp accuracy yi 0.79 a çıkarmıştır

## Discussion :
Hazır kütüphanelerin kullanılması işimizi kolaylaşmıştır. Ayrıca jupyter notebook ortamı hızlıca deney yapmamızı ve sonuçlarını görmemizi sağlamıştır. gridsearch daha dar bir parametre alanında tüm kombinasyonları denememizi sağlar.Random search ise daha geniş bir alanda daha az parametre kombinasyonu denememizi sağlar. ancak gridsearch accuracy yi kötüleştirirken randomsearch in ise pek bir etkisi olmamıştır. PowerTransformer accuracy yi kötüleştirirken QuantileTransformer iyileştirmiştir.
