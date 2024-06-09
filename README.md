
### <div align="center"> Binary (İkili) Sayı Sistemi

Bu tablo, ikili sayı sistemindeki bitlerin, ikili değerlerin, üstel ve ondalık karşılıklarını göstermektedir.

| Bit | Binary (İkili) | Üstel (Exponential) | Ondalık (Decimal) |
|-----|----------------|---------------------|-------------------|
| 0   | 0000           | 2^0                 | 0                 |
| 1   | 0001           | 2^0                 | 1                 |
| 2   | 0010           | 2^1                 | 2                 |
| 3   | 0011           | 2^1 + 2^0           | 3                 |
| 4   | 0100           | 2^2                 | 4                 |
| 5   | 0101           | 2^2 + 2^0           | 5                 |
| 6   | 0110           | 2^2 + 2^1           | 6                 |
| 7   | 0111           | 2^2 + 2^1 + 2^0     | 7                 |
| 8   | 1000           | 2^3                 | 8                 |
| 9   | 1001           | 2^3 + 2^0           | 9                 |
| 10  | 1010           | 2^3 + 2^1           | 10                |

#### Açıklama

İkili sayı sistemi (binary), sadece iki rakam kullanır: 0 ve 1. Her bit, 2'nin farklı bir kuvvetini temsil eder. Tablo, 0'dan 10'a kadar olan ondalık sayıların ikili (binary) karşılıklarını, her bitin 2'nin kuvvetleri cinsinden değerini ve bunların ondalık sistemdeki karşılıklarını gösterir.

- **Bit**: Ondalık (decimal) sistemdeki sayılar.
- **Binary (İkili)**: Her ondalık sayının ikili (binary) sayı sistemindeki temsili.
- **Üstel (Exponential)**: İkili sistemde her bitin 2'nin kuvveti olarak nasıl değerlendirildiği.
- **Ondalık (Decimal)**: İkili sayıların ondalık sistemdeki karşılıkları.

Örneğin, ondalık 5 sayısı ikili sistemde 0101 olarak yazılır. Bu, 2^2 + 2^0 (4 + 1) olarak hesaplanır ve ondalık sistemde 5'e eşittir. Bu sistem, dijital elektronik ve bilgisayar bilimlerinde yaygın olarak kullanılır.


## <div align="center"> IP Adresleri: IPv4 ve IPv6
IPv6, IPv4'ün sınırlamalarını aşmak ve internetin büyüyen ihtiyaçlarını karşılamak için geliştirilmiştir. Özellikle IoT (Internet of Things) gibi uygulamaların artışıyla, IPv6'nın önemi daha da belirginleşmiştir.

#### <div align="center"> IPv4 ve IPv6 Formatları

| Özellik                | IPv4                                        | IPv6                                                   |
|------------------------|---------------------------------------------|--------------------------------------------------------|
| **Adres Uzunluğu**     | 32 bit                                      | 128 bit                                                |
| **Adres Yapısı**       | Dört oktet, 0-255 arası değerler            | Sekiz grup, dört haneli hexadecimal (0-FFFF)           |
| **Temsil**             | Noktalarla ayrılan dört sayı (dotted-decimal notation) | İki nokta üst üste (:) ile ayrılan sekiz grup          |
| **Örnek Adres**        | 192.168.0.1                                  | 2001:0db8:85a3:0000:0000:8a2e:0370:7334                |


#### <div align="center"> IPv4 ve IPv6 Karşılaştırması

| Özellik                 | IPv4                                      | IPv6                                      |
|-------------------------|-------------------------------------------|-------------------------------------------|
| **Adres Uzunluğu**      | 32 bit                                    | 128 bit                                   |
| **Adres Formatı**       | Dört oktet (0-255), noktalarla ayrılmış   | Sekiz grup, dört haneli hexadecimal, iki nokta üst üste (:) ile ayrılmış |
| **Örnek Adres**         | 192.168.0.1                               | 2001:0db8:85a3:0000:0000:8a2e:0370:7334   |
| **Adres Kapasitesi**    | Yaklaşık 4.3 milyar adres                 | 340 undecillion (3.4 x 10^38) adres       |
| **Adres Temsili**       | Ondalık sistem                            | Onaltılık sistem                          |
| **Adres Tükenmesi**     | Sınırlı ve tükenmiş                       | Çok geniş alan, tükenme sorunu yok        |
| **Başlık Yapısı**       | Daha basit ve daha az bilgi içerir        | Daha karmaşık, daha fazla bilgi içerir; optimize edilmiştir |
| **Otomatik Konfigürasyon** | DHCP                                   | SLAAC ve DHCPv6                           |
