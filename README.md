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
