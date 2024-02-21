# RF

RF elektrik ile elektronmanyetik bir alanın etkileşmesi sonucu oluşur. RF dalgalara Elektromanyetik Radyasyon (EMR) denilebilir. Bu elektromanyetik dalgaların başka dalgalar ile karışmasına EMI (Electro Magnetic Interference) denir.

## Frequency Domain (Frekans Bölgesi)
Frekans bölgesi oluşumunda daha çok "Fourier Analizine" başvurulur. Fourier analizi kullanılarak verilen frekanslar daha frekans bölgesinde bulunan daha anlamlı parçalara dönüştürülürler. Bu oluşan dönüşüm sonucunda frekans bölgesinde bulunan 

#### Phase Noise
Osilatör bir periyod boyunca sağladığı frekansı tam olarak koruyamaz bu noktalarda düşüşler ve yükselişler gerçekleşir. Bu duruma Phase Noise denir.

Bazı durumlarda verilen frekansları frekans bölgesinde incelemek için spectrum analyzer denilen cihazlar kullanılır. Osiloskop'un aynı işlevi görmesi için ise cihaz FFT aracılığı ile bu fonksiyonu yerine getirir. Başka bir deyişle Spectrum Analyzer'lar sinyalin frekansı üzerine odaklanırken osiloskoplar ise sinyalin daha çok zaman üzerinde bulunan hareketlerine odaklanırlar.

## dB Birimi Kullanımı

RF tasarımlarında gain olarak kullanılan birim dB olarak tercih edilir çünkü dB 10 üssü olarak logaritmik şekilde kullanılır yani 1000000 gain 60 dB gibi bir şey olmaktadır.

dBm = 1mW
dBW = 1W

dB değerleri ile işlem yapılırken normal toplama çıkarma şeklinde yapılırlar.

dBC -> Sinyalin Gücü

## RF Tasarımında Kullanılan Pasif Komponentler

- Kapasite
- Endüktör
- Direnç
- Kristal
- Anten
- Balun (Transformatör altında incelenirler ama biraz daha farklıdırlar)

## RF Tasarımında Kullanılan Aktif Komponentler

#### Power Amplifier: 
Sinyal Seviyesinin gücünü arttırırlar.

#### LNA(Low Noise Amplifier): 
Bazı durumlarda gönderilen veya alınan sinyallerin büyüklükleri çok düşük olduğu için sinyaller oluşan noislerde kaybolabiliyorlar. Bu nedenle sinyalin bütünlüğünü bozmadan ve fazladan gereksiz şekilde noise oluşturmadan yükseltilmesi gerekmektedir. Bu durumuda devreye LNA'lar girer.

#### RF Mixers:
İki adet input alırlar ve ouptupu kendi aralarında çarpma işlemi yaparak verirler. Bir bakıma inputları translate etmiş olurlar. Mixerlar sinyalleri alçak veya yüksek seviyelere çekebilirler yani değiştirebilirler.

![image](https://github.com/JCDent0n/Electronic_Notes/assets/73293115/bcbe78a3-8ad8-4357-9041-a26086afdb98)

#### Phase-Locked Loops(PLL):
PLL'ler içerisinde Faz dedektörü, Low Pass Filter, Voltaj Kontrollü Osilatör, Frekans Bölücü gibi parçalar barındıran bir componenttir (Yani bir çoğunda bu parçalar bulunur). Osilatör yardımı ile beraber kullanıldığı zaman ihtiyacımız olana farklı seviyelerde frekans üretimi konusunda büyük yardımcı olurlar.

![image](https://github.com/JCDent0n/Electronic_Notes/assets/73293115/4bb0bba3-acd6-4ec5-aaff-6f7fd9ffa7e1)


#### Data Converters:
Bunlara basit örnek ADC'ler veya DAC'lerdir.

## Frekans Tipleri

Birden Fazla frekans tipi vardır bunların devre tasarımında kullanılanlardan bir kaçı;

- LF(Low Frequency)
- MF(Medium Frequency)
- HF(High Frequency)
- VHF(Very High Frequency)
- UHF(Ultra High Frequency)
- SHF(Super High Frequency)

![image](https://github.com/JCDent0n/Electronic_Notes/assets/73293115/b741c644-a8dc-4e2c-8bd1-42308330b9fe)
