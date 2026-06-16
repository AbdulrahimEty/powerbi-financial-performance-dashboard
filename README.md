Finansal Performans Dashboard'u (Power BI)

Microsoft'un Financial Sample veri setini kullanarak yaptığım, 2 sayfalık bir Power BI dashboard'u. Power BI ve DAX öğrenme sürecimde portföyüme eklediğim bir proje.


İçerik

Sayfa 1:


5 KPI kartı (Net Satış, Toplam Kâr, Kâr Marjı, Satılan Adet, İndirim Oranı)
Aylık gelir & kâr trendi (çizgi grafik)
Ülke bazında satış (yatay bar)
Segment dağılımı (halka grafik)
Ürün bazında satış & kâr (sütun grafik)
Yıl filtresi


Sayfa 2:


5 KPI kartı (Brüt Satış, Maliyet, Brüt Kâr, Ort. Satış Fiyatı, Sipariş Adedi)
Ürün × Segment kârlılık matrisi (renk skalalı)
İndirim - kâr ilişkisi (scatter chart)
Segment bazında kâr katkısı (waterfall)


Kullandığım Şeyler


Power BI Desktop
DAX (SUM, CALCULATE, SUMX, DIVIDE, DISTINCTCOUNT)
Power Query (veri tipi düzeltme)
PowerPoint (arka plan tasarımı)


Yazdığım DAX Ölçüleri

daxNet Satış      = SUM(financials[Sales])
Toplam Kâr     = SUM(financials[Profit])
Kâr Marjı      = DIVIDE([Toplam Kâr], [Net Satış])
Brüt Kâr       = [Brüt Satış] - [Toplam Maliyet]
Sipariş Adedi  = COUNT(financials[Sales])

Tasarım Notları


Lacivert + turuncu palet (Corporate Navy)
PowerPoint'te 1920×1080 arka plan
KPI'lar üstte, grafikler altta — Z-pattern


Veri Seti

Microsoft Financial Sample — 700 satır, 16 sütun.

İndirme linki

Dosyalar

├── README.md
├── Finansal_Performans_Dashboard.pbix
├── images/
│   ├── sayfa1.png
│   └── sayfa2.png
└── data/
    └── Financial_Sample.xlsx


Abdülrahim Etyemez

LinkedIn
