# SarcasmDetection
Sarcasm Detection'daki geçmiş çalışmalar çoğunlukla hashtag tabanlı denetim kullanılarak toplanan Twitter veri kümelerini kullanır, ancak bu tür veri kümeleri etiketler
ve dil açısından gürültülüdür. Ayrıca, birçok tweet, diğer tweet'lere yanıttır ve bunlarda alaycılığı tespit etmek, bağlamsal tweet'lerin kullanılabilirliğini gerektirir.
Twitter veri kümelerindeki gürültüyle ilgili sınırlamaların üstesinden gelmek için, Sarcasm Detection için bu Başlıklar veri kümesi iki haber web sitesinden toplanmıştır. TheOnion , güncel olayların alaycı versiyonlarını üretmeyi hedefliyor ve tüm manşetleri Kısa Haberler ve Fotoğraflarda Haberler (alaycı olan) kategorilerinde topladık. HuffPost'tan gerçek (ve alaycı olmayan) haber başlıkları topluyoruz .
Bu yeni veri kümesi, mevcut Twitter veri kümelerine göre aşağıdaki avantajlara sahiptir:
Haber manşetleri profesyoneller tarafından resmi bir şekilde yazıldığı için yazım yanlışları ve resmi olmayan kullanımlar söz konusu değildir. Bu, seyrekliği azaltır ve ayrıca önceden eğitilmiş yerleştirmeleri bulma şansını artırır.
Ayrıca TheOnion'un tek amacı alaycı haberler yayınlamak olduğundan, Twitter veri kümelerine kıyasla çok daha az gürültülü, yüksek kaliteli etiketler elde ediyoruz.
Diğer tweetlere verilen yanıtlardan farklı olarak, elde ettiğimiz haber başlıkları bağımsızdır. Bu, gerçek alaycı unsurları ayırmamıza yardımcı olacaktır.
Hangi haberlerin alaycı, hangilerinin olmadığını bulmamız gerekiyor. Bu sorun iki görevde çözüldü.

• Verileri okuyun ve temizleyin
• En yaygın sözcükleri bulun ve görselleştirin
• Durdurulan sözcükleri belirleyin ve görselleştirin
• Metni ön işlemden geçirin
• Sınıflandırma modellerini tanımlayın
• En iyi modeli alın ve kaydedin

2 görevde aşağıdaki planla çalışıldı:

• Verileri yükleyin ve ön işleme tabi tutun
• Derin Öğrenme modellerini tanımlayın
• Sorunu çözmek için en iyi modeli alın
• Modeli kaydedin.
**

Elimizde iki haber sitesinden alaycı manşetlerden oluşan bir veri setimiz var. Üç öznitelikten oluşan her veri kümesi vardır:

- is_sarcastic: 1 if the dataset is sarcastic, 0 otherwise
- headline: the headline of the news article
- article_link: Link to the original news article.
