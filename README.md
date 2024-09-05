# İçindekiler

- [Binary (İkili) Sayı Sistemi](#binary-ikili-sayi-sistemi)
   - [Açıklama](#açıklama)
- [IP Adresleri: IPv4 ve IPv6](#ip-adresleri-ipv4-ve-ipv6)
   - [IPv4 ve IPv6 Formatları](#ipv4-ve-ipv6-formatları)
   - [IPv4 ve IPv6 Karşılaştırması](#ipv4-ve-ipv6-karşılaştırması)
- [IP Adres Sınıfları](#ip-adres-sınıfları)
   - [A Sınıfı IP Adresi](#a-sınıfı-ip-adresi)
   - [B Sınıfı IP Adresi](#b-sınıfı-ip-adresi)
   - [C Sınıfı IP Adresi](#c-sınıfı-ip-adresi)
   - [D Sınıfı IP Adresi](#d-sınıfı-ip-adresi)
   - [E Sınıfı IP Adresi](#e-sınıfı-ip-adresi)
- [IP Adres Sınıfları ve Hesaplamaları](#ip-adres-sınıfları-ve-hesaplamaları)
- [IP Hesaplamaları](#ip-hesaplamaları)
   - [Alt Ağ (Subnet) Hesaplaması](#alt-ağ-subnet-hesaplaması)
   - [Alt Ağ Maskesi](#alt-ağ-maskesi)
   - [CIDR Notasyonu](#cidr-notasyonu)
   - [Kullanılabilir IP Sayısı Hesaplaması](#kullanılabilir-ip-sayısı-hesaplaması)
   - [Wildcard Maskesi](#wildcard-maskesi)
- [Örnek Hesaplamalar](#örnek-hesaplamalar)


<h2 id="binary-ikili-sayi-sistemi" align="center">Binary (İkili) Sayı Sistemi</h2>

Bu tablo, ikili sayı sistemindeki bitlerin, ikili değerlerin, üstel ve ondalık karşılıklarını göstermektedir.

---

<div align="center">
  <table>
    <tr>
      <th>Bit</th>
      <th>Binary (İkili)</th>
      <th>Üstel (Exponential)</th>
      <th>Ondalık (Decimal)</th>
      <th>Bit</th>
      <th>Binary (İkili)</th>
      <th>Üstel (Exponential)</th>
      <th>Ondalık (Decimal)</th>
    </tr>
    <tr>
      <td>0</td>
      <td>0000</td>
      <td>2^0</td>
      <td>0</td>
      <td>6</td>
      <td>0110</td>
      <td>2^2 + 2^1</td>
      <td>6</td>
    </tr>
    <tr>
      <td>1</td>
      <td>0001</td>
      <td>2^0</td>
      <td>1</td>
      <td>7</td>
      <td>0111</td>
      <td>2^2 + 2^1 + 2^0</td>
      <td>7</td>
    </tr>
    <tr>
      <td>2</td>
      <td>0010</td>
      <td>2^1</td>
      <td>2</td>
      <td>8</td>
      <td>1000</td>
      <td>2^3</td>
      <td>8</td>
    </tr>
    <tr>
      <td>3</td>
      <td>0011</td>
      <td>2^1 + 2^0</td>
      <td>3</td>
      <td>9</td>
      <td>1001</td>
      <td>2^3 + 2^0</td>
      <td>9</td>
    </tr>
    <tr>
      <td>4</td>
      <td>0100</td>
      <td>2^2</td>
      <td>4</td>
      <td>10</td>
      <td>1010</td>
      <td>2^3 + 2^1</td>
      <td>10</td>
    </tr>
    <tr>
      <td>5</td>
      <td>0101</td>
      <td>2^2 + 2^0</td>
      <td>5</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
  </table>
</div>

---

#### Açıklama

İkili sayı sistemi (binary), sadece iki rakam kullanır: 0 ve 1. Her bit, 2'nin farklı bir kuvvetini temsil eder. Tablo, 0'dan 10'a kadar olan ondalık sayıların ikili (binary) karşılıklarını, her bitin 2'nin kuvvetleri cinsinden değerini ve bunların ondalık sistemdeki karşılıklarını gösterir.

- **Bit**: Ondalık (decimal) sistemdeki sayılar.
- **Binary (İkili)**: Her ondalık sayının ikili (binary) sayı sistemindeki temsili.
- **Üstel (Exponential)**: İkili sistemde her bitin 2'nin kuvveti olarak nasıl değerlendirildiği.
- **Ondalık (Decimal)**: İkili sayıların ondalık sistemdeki karşılıkları.

Örneğin, ondalık 5 sayısı ikili sistemde 0101 olarak yazılır. Bu, 2^2 + 2^0 (4 + 1) olarak hesaplanır ve ondalık sistemde 5'e eşittir. Bu sistem, dijital elektronik ve bilgisayar bilimlerinde yaygın olarak kullanılır.

---

## <div align="center">IP Adresleri: IPv4 ve IPv6
IPv6, IPv4'ün sınırlamalarını aşmak ve internetin büyüyen ihtiyaçlarını karşılamak için geliştirilmiştir. Özellikle IoT (Internet of Things) gibi uygulamaların artışıyla, IPv6'nın önemi daha da belirginleşmiştir.

---

#### <div align="center">IPv4 ve IPv6 Formatları

| Özellik                | IPv4                                        | IPv6                                                   |
|------------------------|---------------------------------------------|--------------------------------------------------------|
| **Adres Uzunluğu**     | 32 bit                                      | 128 bit                                                |
| **Adres Yapısı**       | Dört oktet, 0-255 arası değerler            | Sekiz grup, dört haneli hexadecimal (0-FFFF)           |
| **Temsil**             | Noktalarla ayrılan dört sayı (dotted-decimal notation) | İki nokta üst üste (:) ile ayrılan sekiz grup          |
| **Örnek Adres**        | 192.168.0.1                                  | 2001:0db8:85a3:0000:0000:8a2e:0370:7334                |

---

#### <div align="center">IPv4 ve IPv6 Karşılaştırması

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

---

### <div align="center">IP Adres Sınıfları

Bu tablo, IP adreslerinin sınıflarını ve her sınıfın özelliklerini göstermektedir.

| Sınıf | Başlangıç Adresi | Bitiş Adresi   | Alt Ağ Maskesi       | Ağ Sayısı  | Her Ağda Maksimum Host Sayısı | Kullanım Alanı         |
|-------|------------------|----------------|----------------------|------------|-------------------------------|------------------------|
| A     | 0.0.0.0          | 127.255.255.255| 255.0.0.0 (/8)       | 128        | 16,777,214                    | Büyük ağlar            |
| B     | 128.0.0.0        | 191.255.255.255| 255.255.0.0 (/16)    | 16,384     | 65,534                        | Orta büyüklükte ağlar   |
| C     | 192.0.0.0        | 223.255.255.255| 255.255.255.0 (/24)  | 2,097,152  | 254                           | Küçük ağlar            |
| D     | 224.0.0.0        | 239.255.255.255| Kullanılmaz          | Kullanılmaz| Kullanılmaz                   | Multicast              |
| E     | 240.0.0.0        | 255.255.255.255| Kullanılmaz          | Kullanılmaz| Kullanılmaz                   | Deneysel, araştırma    |

IP adresleri, ağları daha verimli yönetmek için sınıflara ayrılmıştır. Bu sınıflar, ağın büyüklüğüne ve kullanım amacına göre farklılık gösterir. A, B ve C sınıfları, farklı büyüklükteki ağlar için uygundur, D sınıfı multicast için kullanılırken, E sınıfı ise deneysel amaçlar için ayrılmıştır.

### Açıklama:

- #### A Sınıfı IP Adresi
  - Büyük ağlar için kullanılır. İlk oktet (0-127) ağ adresini belirtir.
  - **Örnek Adres:** 10.0.0.1
  - **Açıklama:** 10.0.0.1, A sınıfı bir IP adresidir. A sınıfı IP adresleri, büyük ağlarda kullanılır ve geniş bir adres aralığına sahiptir. İlk oktet (10), ağ adresini belirtir, geri kalan üç oktet (0.0.1) ise host adresini belirtir.
  - **Kullanılabilir Aralık:** 1.0.0.0 - 126.255.255.255

     <img src="https://i.hizliresim.com/610q84w.PNG" alt="IP Address Example" width="650" height="350">

- #### B Sınıfı IP Adresi
  - Orta büyüklükteki ağlar için kullanılır. İlk iki oktet (128-191) ağ adresini belirtir.
  - **Örnek Adres:** 172.16.0.1
  - **Açıklama:** 172.16.0.1, B sınıfı bir IP adresidir. B sınıfı IP adresleri, orta büyüklükteki ağlarda kullanılır. İlk iki oktet (172.16) ağ adresini, geri kalan iki oktet (0.1) ise host adresini belirtir.
  - **Kullanılabilir Aralık:** 128.0.0.0 - 191.255.255.255

      <img src="https://i.hizliresim.com/ggovdpf.PNG" alt="IP Address Example" width="650" height="350">

- #### C Sınıfı IP Adresi
  - Küçük ağlar için kullanılır. İlk üç oktet (192-223) ağ adresini belirtir.
  - **Örnek Adres:** 192.168.1.1
  - **Açıklama:** 192.168.1.1, C sınıfı bir IP adresidir. C sınıfı IP adresleri, küçük ağlarda kullanılır. İlk üç oktet (192.168.1) ağ adresini, son oktet (1) ise host adresini belirtir.
  - **Kullanılabilir Aralık:** 192.0.0.0 - 223.255.255.255

      <img src="https://i.hizliresim.com/slfe9pz.PNG" alt="IP Address Example" width="650" height="350">

- #### D Sınıfı IP Adresi
  - Multicast adresleme için kullanılır. Ağ adresleme için kullanılmaz.
  - **Örnek Adres:** 224.0.0.1
  - **Açıklama:** 224.0.0.1, D sınıfı bir IP adresidir. D sınıfı IP adresleri, multicast iletişimde kullanılır. Bu adresler, ağ üzerindeki belirli cihaz gruplarına veri göndermek için kullanılır.
  - **Aralık:** 224.0.0.0 - 239.255.255.255

      <img src="https://i.hizliresim.com/ktzrup7.PNG" alt="IP Address Example" width="650" height="350">

- #### E Sınıfı IP Adresi
  - Deneysel amaçlar için ayrılmıştır. Ağ adresleme için kullanılmaz.
  - **Örnek Adres:** 240.0.0.1
  - **Açıklama:** 240.0.0.1, E sınıfı bir IP adresidir. E sınıfı IP adresleri, deneysel ve araştırma amaçlı kullanılır. Bu adresler, genellikle özel amaçlar için ayrılmıştır ve normal ağ iletişiminde kullanılmaz.
  - **Aralık:** 240.0.0.0 - 255.255.255.255

      <img src="https://i.hizliresim.com/b6huzu3.PNG" alt="IP Address Example" width="650" height="250">

  ---

### <div align="center">IP Adres Sınıfları ve Hesaplamaları

IP adresleri, ağların büyüklüğüne ve kullanımına göre sınıflandırılmıştır. Her sınıfın farklı adres aralıkları, alt ağ maskeleri ve hesaplama yöntemleri bulunur.

| Sınıf | Başlangıç Adresi | Bitiş Adresi   | Alt Ağ Maskesi       | Ağ Sayısı  | Her Ağda Maksimum Host Sayısı | Kullanım Alanı         |
|-------|------------------|----------------|----------------------|------------|-------------------------------|------------------------|
| A     | 0.0.0.0          | 127.255.255.255| 255.0.0.0 (/8)       | 128        | 16,777,214                    | Büyük ağlar            |
| B     | 128.0.0.0        | 191.255.255.255| 255.255.0.0 (/16)    | 16,384     | 65,534                        | Orta büyüklükte ağlar   |
| C     | 192.0.0.0        | 223.255.255.255| 255.255.255.0 (/24)  | 2,097,152  | 254                           | Küçük ağlar            |
| D     | 224.0.0.0        | 239.255.255.255| Kullanılmaz          | Kullanılmaz| Kullanılmaz                   | Multicast              |
| E     | 240.0.0.0        | 255.255.255.255| Kullanılmaz          | Kullanılmaz| Kullanılmaz                   | Deneysel, araştırma    |

---

### <div align="center">IP Hesaplamaları

#### **Alt Ağ (Subnet) Hesaplaması**
Alt ağlar, bir IP adresi blokunu daha küçük ağlara bölmek için kullanılır. Subnetting yapıldığında ağ ID'si ve host ID'si belirlenir. 

**Örnek:**  
Bir ağ 192.168.1.0/24 IP bloğunu kullanıyorsa:
- Alt Ağ Maskesi: 255.255.255.0
- İlk IP Adresi (Ağ ID'si): 192.168.1.0
- Son IP Adresi (Broadcast): 192.168.1.255
- Kullanılabilir IP aralığı: 192.168.1.1 - 192.168.1.254 (Toplam 254 host)

#### **Alt Ağ Maskesi**
Alt ağ maskesi, ağın ve host kısmını ayırt etmek için kullanılır. CIDR notasyonu (/24, /16 vb.) bu maskeyi belirtir.

**Örnek:**
- **/24** Alt ağ maskesi: 255.255.255.0 
- **/16** Alt ağ maskesi: 255.255.0.0

#### **CIDR Notasyonu**
CIDR (Classless Inter-Domain Routing), IP adreslerini ve alt ağları daha esnek bir şekilde belirtir.

**Örnek:**  
192.168.1.0/24, 256 IP adresini temsil eder ve alt ağ maskesi 255.255.255.0'dır.

#### **Kullanılabilir IP Sayısı Hesaplaması**
Herhangi bir alt ağda kullanılabilir IP adresi sayısı şu formülle hesaplanır:  
`Kullanılabilir IP = 2^(32 - CIDR) - 2`

**Örnek:**
- /24 için: 2^(32 - 24) - 2 = 256 - 2 = 254 kullanılabilir IP
- /16 için: 2^(32 - 16) - 2 = 65,536 - 2 = 65,534 kullanılabilir IP

#### **Wildcard Maskesi**
Wildcard maskesi, alt ağ maskesinin tersidir ve genellikle ACL (Access Control List) gibi güvenlik kurallarında kullanılır.

**Örnek:**
- Alt ağ maskesi 255.255.255.0 için wildcard maskesi: 0.0.0.255

---

### Örnek Hesaplamalar

**Ağ:** 192.168.1.0/24  
- Alt Ağ Maskesi: 255.255.255.0
- CIDR Notasyonu: /24
- Kullanılabilir IP Aralığı: 192.168.1.1 - 192.168.1.254
- Broadcast Adresi: 192.168.1.255
- Toplam Host Sayısı: 254

**Ağ:** 10.0.0.0/8  
- Alt Ağ Maskesi: 255.0.0.0
- CIDR Notasyonu: /8
- Kullanılabilir IP Aralığı: 10.0.0.1 - 10.255.255.254
- Broadcast Adresi: 10.255.255.255
- Toplam Host Sayısı: 16,777,214

