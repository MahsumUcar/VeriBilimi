# Makine Öğreniminde K-means

K-means kümeleme, K-means algoritması, K-means kümeleme algoritması - yani, kümelemenin neyle ilgili olduğuna dalmadan önce, modern zaman işletmelerinin verileri anlamlandırmasının ne kadar önemli olduğunu anlamamız gerekiyor - ürünlerle ilgili veriler, müşterilerle ilgili veriler, işlemlerle ilgili veriler vb.

Teknolojinin iş ortamını yeniden tanımladığı bir dünyada işletmeler, daha verimli olmalarına ve karlarını artırmalarına yardımcı olacak modeller bulmak için verileri analiz ederek milyonlarca dolar harcıyor. Nesneleri niteliklere göre gruplandırmak, bu tür kalıpları ortaya çıkarma sürecinde yer alan ilk görevlerden biridir.

Nesneleri gruplamak, kuruluşların çeşitli durumlar için çeşitli stratejiler tasarlamasına yardımcı olur. Müşteriler, ürünler ve işlemler, bu tür süreçlerde temel ilgi alanlarıdır. Müşterileri davranışlarına göre gruplamak, işletmelerin kişiselleştirilmiş teklifler tasarlamasına yardımcı olur. Ürünleri gruplamak, müşterilere alternatif seçenekler sunmalarına yardımcı olur. Ve işlemleri gruplamak, daha yakından dikkat gerektiren olağandışı kalıpları belirlemelerine yardımcı olur.

Kümelemenin devreye girdiği yer burasıdır. Kümeleme temel olarak nesneleri niteliklere göre gruplandıran denetimsiz bir makine öğrenimi (ML) algoritmasıdır.

Üretime hazır yapay zeka için lider bir vektör veritabanı şirketi olan Zilliz'in bu kapsamlı makalesi, sizi K'nin makine öğreniminde kümelemenin ne anlama geldiğini ve Python kullanarak bunu nasıl uygulayabileceğinizi derinlemesine ele alacak.

# Kümeleme Nedir?
Belirli bir gruptaki her öğe, diğer gruplardaki öğelere göre o gruptaki öğelere daha benzer olacak şekilde veri noktalarını gruplama işlemidir.

Kümeleme, belirli bir algoritmaya atıfta bulunmaz. Birçok algoritma kullanılarak çözülebilen genel bir görevdir. Kümeleme algoritmaları genellikle benzerliği sistematik olarak ölçmek için bir ölçü tanımlar. Kümeleme, görüntü işleme, bilgi alma, öneri motorları, veri sıkıştırma vb. birçok alanda kullanılmaktadır.

Kümeleme, kümelediği nesnelerin özelliklerine göre benzerlik kurar. Nitelikler etki alanına göre farklılık gösterir. Örneğin, bir görüntü söz konusu olduğunda, nitelikler piksel değerleridir. Bir kullanıcı profili söz konusu olduğunda, nitelikler yaş, cinsiyet, satın alma geçmişi vb. ayrıntılardır. Bir ürün söz konusu olduğunda, nitelikler kategori, renk, fiyat vb.

Kümeleme, denetimsiz bir görev olarak adlandırılır çünkü etiketli verilerin hazırlanmasını içeren, kullanıcı tarafından izlenen bir eğitim süreci yoktur.

#Kümeleme Algoritmaları Nasıl Çalışır?

Çoğu kümeleme algoritması, tüm örnek çiftleri arasındaki benzerliği hesaplayarak çalışır. Benzerliğin hesaplanma şekli ve ikili benzerliğin hesaplanma sırası, kümeleme algoritmasının türüne göre değişir.

Veri kümesinin hacmi için ölçeklendirme yeteneği, bir problem için kümeleme algoritmasına karar verirken göz önünde bulundurulması gereken önemli bir faktördür. Yürütme süresi, eleman çiftlerinin sayısı ile artar. Aşırı durumlarda, veri hacminin karesiyle orantılı olarak değişebilir.


# Kümeleme Yaklaşımları
Kümeleme için dört yaygın yaklaşım vardır: ağırlık merkezi tabanlı, yoğunluk tabanlı, hiyerarşik ve dağıtım tabanlı. Tek tek onlara bir göz atalım.

1. Centroid Tabanlı Kümeleme
Bu yöntem, veri noktalarını, kümenin merkezine dayalı olarak herhangi bir hiyerarşi olmadan ayrı kümeler halinde düzenler. Centroid, bir nesnenin geometrik merkezidir. Basit bir ifadeyle, n-boyutlu uzayda o cismi oluşturan tüm noktaların aritmetik ortalamasıdır. Burada bir küme, bir merkezin etrafında bulunan noktaların bir koleksiyonudur. Centroid tabanlı kümeleme, ilk atamalar ve aykırı değerlerle ilgili sorunlardan muzdariptir.

2. Yoğunluk Tabanlı Kümeleme
Adından da anlaşılacağı gibi, bir alandaki noktaların yoğunluğunu hesaplar ve yüksek yoğunluğun bulunduğu her yere kümeler atar. Bu durumda, kümeler herhangi bir şekil alabilir. Yoğunluğa dayalı kümeleme, verilerin doğası gereği yoğunlukta yüksek bir varyansa sahip olduğunda sorunlarla karşılaşır. Veri boyutu yüksek olduğunda iyi performans göstermez.

3. Hiyerarşik Kümeleme
Bu yöntem, daha büyük kümeler içinde yer alan kümeler olasılığına sahip bir küme ağacı sağlar. Bu yöntem, veriler içsel bir hiyerarşi sergilediğinde iyi bir uyum sağlar. Hiyerarşik kümeleme, uygulamadan sonra herhangi bir sayıda kümenin seçilmesine izin verir, çünkü analist gerekli noktada ağacı kırabilir ve yalnızca bu noktadan sonraki kümeleri dikkate alabilir.

4. Dağıtım Tabanlı Kümeleme
Bu yöntem, kümeleri bulmak için olasılık dağılımları kavramını kullanır. Merkezden uzaklaştıkça bir noktanın kümede olma olasılığının azaldığını varsayar. Geliştiriciler, bu yöntemi etkili bir şekilde kullanmak için verilerinin dağıtımını bilmelidir.




