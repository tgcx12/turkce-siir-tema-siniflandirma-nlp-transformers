
# 🎓 Türkçe Şiirlerin Tematik Sınıflandırılması — NLP + Transformer Modeller

Bu proje kapsamında Türkçe şiirler; **aşk, gurbet, kahramanlık, pastoral ve tasavvuf** olmak üzere beş farklı temaya göre sınıflandırılmıştır. Çalışmada modern Doğal Dil İşleme (NLP) yöntemleri ve Transformer tabanlı modeller (BERT, ELECTRA, DeBERTa, XLM-R, ALBERT) kullanılmıştır.

## 🧠 Amaç
Şiir gibi edebi yoğunluğu yüksek metinlerde tematik ayrım yaparak, anlam katmanlarını makine öğrenmesiyle çözümlemeye çalışmak. Bu kapsamda sınıflandırma doğruluğu yüksek, overfitting'e karşı dirençli ve Türkçe ile uyumlu modeller denenmiştir.

## 🧪 Kullanılan Modeller
- Microsoft/DeBERTa-base
- dbmdz/Electra-base-Turkish-cased
- xlm-roberta-base
- albert-base-v2
- bert-base-turkish-cased

## 🗃️ Veri ve Ön İşleme
- Web scraping ile derlenmiş Türkçe şiirler
- Lemmatization, stopword temizliği, lowercasing
- Data augmentation: [TextAttack](https://www.analyticsvidhya.com/blog/2022/02/text-data-augmentation-in-natural-language-processing-with-texattack/)

## ⚙️ Eğitim Süreci
- Eğitim Colab üzerinde GPU ile gerçekleştirilmiştir
- Eğitim süresince `early stopping`, `label smoothing`, `weight decay`, `warmup` gibi stratejiler uygulanmıştır
- ROC eğrisi, karmaşıklık matrisi ve metrikler karşılaştırılarak en uygun model belirlenmiştir

## 📊 Sonuçlar
| Model        | Accuracy | F1 Skoru | Eğitim Süresi |
|--------------|----------|----------|----------------|
| DeBERTa      | 96.41%   | 0.9641   | 10,918 sn      |
| ELECTRA      | 95.37%   | 0.9537   | 3,870 sn       |
| Diğerleri    | README sonunda detaylı grafikte | | 

## 📎 Rapor
Ayrıntılı rapora aşağıdaki bağlantıdan ulaşabilirsiniz:  
[Projeyi Anlatan PDF Raporunu Görüntüle](./Tuğçe_Gül_221307036%20(1).pdf)


## 📚 Kaynakça
- [Text Data Augmentation with TextAttack](https://www.analyticsvidhya.com/blog/2022/02/text-data-augmentation-in-natural-language-processing-with-texattack/)
- [Doğal Dil İşleme Nedir – Merve Enoyan](https://merveenoyan.medium.com/do%C4%9Fal-dil-i%CC%87%C5%9Fleme-natural-language-processing-2d7c72daf245)
- [Google Colab](https://colab.research.google.com)

---

📌 Bu projede kullanılan yöntemler, Türkçe gibi düşük kaynaklı dillerde şiirsel metinlerin sınıflandırılmasına örnek teşkil etmektedir.

