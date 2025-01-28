# Kuzey Kıbrıs NO2 Kirliliği Analizi: Teknecik ve Kalecik Bölgeleri (2019-2025)

Bu GitHub deposu, Kuzey Kıbrıs'ta bulunan Teknecik ve Kalecik bölgelerindeki atmosferik azot dioksit (NO2) kirliliğinin analizine yönelik bir çalışma için kullanılan kodları, verileri ve diğer ilgili materyalleri içermektedir. Bu çalışma, 2019 yılından 18 Ocak 2025 tarihine kadar olan uydu verilerini kullanarak, bölgedeki NO2 seviyelerini değerlendirmeyi amaçlamaktadır.

## Proje Amacı

Bu proje, şu amaçları gütmektedir:

*   Kuzey Kıbrıs'ta bulunan Teknecik ve Kalecik bölgelerindeki NO2 kirliliğinin düzeyini belirlemek.
*   NO2 seviyelerinin aylık, yıllık ve mevsimsel değişimlerini analiz etmek.
*   Aykırı (anormal yüksek veya düşük) NO2 değerlerini tespit etmek ve bu değerlerin dağılımını incelemek.
*   Her iki bölgedeki NO2 kirliliğini karşılaştırmak.
*   Elde edilen sonuçları kullanarak halkı bilinçlendirmek ve politika yapıcıları harekete geçirmek.
*   Çalışmanın tüm aşamalarını şeffaf bir şekilde paylaşarak diğer araştırmacılar için referans bir kaynak oluşturmak.
*   Veri,  Google Earth Engine platformundan elde edilen "OPERNICUS/S5P/OFFL/L3_NO2" imajları kullanılarak 10.000 metre radyusluk bir alanda örneğin Teknecik için haritada çizilmiş alan için NO2 değerleri ortalaması alınarak elde edilmiştir.

## İçerik

Bu depo aşağıdaki dosyaları içermektedir:

*   **`Daily_NO2_Teknecik_2019-202501.csv`:** Teknecik bölgesine ait günlük NO2 değerlerini içeren CSV dosyası. (2019-01-01 ile 2025-01-18 aralığını kapsar)
*   **`Daily_NO2_Kalecik_2019-202501.csv`:** Kalecik bölgesine ait günlük NO2 değerlerini içeren CSV dosyası. (2019-01-01 ile 2025-01-18 aralığını kapsar)
*   **`NO2_Analysis_Teknecik_Kalecik.ipynb`:** Tüm analizleri, veri işleme adımlarını ve grafikleri içeren Colab notebook dosyası.
*  **`input.png`** Makalede kullanılan harita görseli.
*  **`File_input_1.png`** Teknecik aylık ortalama NO2 grafiği.
*  **`File_input_1_2.png`** Teknecik yıllık ortalama NO2 grafiği.
*  **`File_input_2.png`** Kalecik aylık ortalama NO2 grafiği.
*  **`File_input_2_2.png`** Kalecik yıllık ortalama NO2 grafiği.
*  **`File_input_3.png`** Aykırı değerler karşılaştırma grafiği.
*   **`File_input_4.png`** Yıllık ortalama NO2 değerleri karşılaştırma grafiği.
*   **`README.md`:** Bu dosya (proje hakkında genel bilgileri içerir).

## Kullanılan Teknolojiler

*   **Python:** Veri analizi ve görselleştirme için kullanılan programlama dili.
*   **pandas:** Veri işleme ve manipülasyon için kullanılan Python kütüphanesi.
*   **matplotlib:** Veri görselleştirme için kullanılan Python kütüphanesi.
*   **Google Colab:** Python kodlarının yürütüldüğü bulut tabanlı platform.
*   **Google Earth Engine:** Uydu verilerinin elde edildiği platform.

## Analiz Adımları

1.  **Veri Toplama:** Google Earth Engine üzerinden uydu verileri indirilmiştir. Veriler, "OPERNICUS/S5P/OFFL/L3_NO2" imajlarından elde edilmiştir.
2.  **Veri İşleme:**
    *   Günlük NO2 değerleri, her iki bölge için ayrı ayrı CSV dosyalarına kaydedilmiştir.
    *   Python ve pandas kütüphanesi kullanılarak veriler düzenlenmiş ve temizlenmiştir.
    *   Tarih sütunları, analiz için uygun formata getirilmiştir.
3.  **Veri Analizi:**
    *   Her iki bölge için aylık, yıllık ve mevsimsel ortalama NO2 seviyeleri hesaplanmıştır.
    *   Standart sapma, minimum ve maksimum değerler belirlenmiştir.
    *   Aykırı değerler (IQR yöntemiyle) tespit edilmiştir.
    *   Her iki bölgenin NO2 seviyeleri karşılaştırmalı olarak analiz edilmiştir.
    *   Analiz sonuçları grafiklerle ve tablolarla görselleştirilmiştir.
4.  **Sonuç ve Yorumlama:**
    *   Elde edilen sonuçlar, bilimsel olarak yorumlanarak makalede sunulmuştur.

## Colab Notebook'u Çalıştırma

*   Bu depodaki `NO2_Analysis_Teknecik_Kalecik.ipynb` dosyasını kullanarak analizleri tekrar edebilirsiniz.
*   Google Colab ortamında notebook'u açın.
*   Gerekli Python kütüphanelerinin yüklü olduğundan emin olun (pandas, matplotlib).
*   Notebook'daki tüm kod hücrelerini sırayla çalıştırın.
*   Sonuçlar ve grafikler notebook içerisinde görüntülenecektir.

## Katkı ve Geri Bildirim

*   Bu projeye katkıda bulunmak isterseniz, pull request gönderebilir veya hataları/önerilerinizi issues olarak bildirebilirsiniz.
*   Çalışma hakkında geri bildirimlerinizi ve sorularınızı memnuniyetle karşılarım.

## Lisans

Bu proje, MIT lisansı ile lisanslanmıştır.
