---
page_title: Politikalar ve Eklentiler
title: Liman MYS'de Politikalar
include_footer: true
---

<!--{{% title3 "§1 Lorem" %}}-->
Linux işletim sistemine sahip istemcileri ve kullanıcıları belirlenen ve ihtiyaç duyulan kurallara bağlı olarak olarak uzaktan merkezi olarak yönetme imkanı sağlar. Politikilarımız özellikle BT işletimini gerçekleştiren sistem yöneticilerinin ihtiyaçları tespit edilerek geliştirilmiştir. Politikalarımız ile kullanıcılarınızın, istemcilerinizin, sunucularınızın güncel, stabil ve güvenilir olmasını sağlarsınız.
<br><br>
{{% liman-image-viewer "politikalar-ve-eklentiler/liman-mys-genis-petek.jpg" "is-three-quarters" %}}
<hr>
{{% title3 "Eklentiler" %}}<div class="divider" style="margin-top: -20px; margin-bottom: 20px;"></div>

Liman MYS, eklentileri aracılığıyla Linux ve Windows sunucuları yönetir. Eklentiler mimarisi framework methoduyla çalışır, bu sebepten belirlenen ihtiyaçlar kadar Liman MYS‘nin kabiliyetlerini genişletebilirsiniz. Eklentileri uzak sunucuları yönetmek, log kaydı yapmak ve belirlenen görevleri yerine getirmek olduğu için Liman MYS üzerinde hiç bir şekilde veri tutulmaz, yönetimi sağlanan mevcut sunucuların verileri kullanılır. Bu sebeple, Liman MYS mevcut sistemlere down time korkusu olmadan entegre olur.
<br><br>
<hr>

{{% title4 "Domain Eklentisi" %}}

Aktif Dizin ya da Samba Domain sunucularının yönetildiği eklentidir. Kullanici, grup, istemci ve politika objelerini yönetebilir, Linux istemcilerine politika uygulatabilir; Pardus, Debian, Linux Mint, CentOS ve MacOS işletim sistemine sahip cihazlari <b>uzaktan mevcut domaininize dahil edebilirsiniz</b>.
<br><br><br>
{{% liman-image-viewer "illustrations/liman_arayuz_resim.png" %}}
<br><br>
<hr>
{{% title4 "Jitsi Eklentisi" %}}

Pardus ve Ubuntu tabanlı sunucularınıza Jitsi kurulumunu uzaktan gerçekleştirebilirsiniz. LDAP konfigürasyonu ile Jitsi odalarına yalnizca domain kullanıcılarının dahil olmasını sağlayabilirsiniz. Jitsi üzerinde konfigürasyon ayarları yaparak performans artışı sağlayabilir, arayüzünü düzenleyebilirsiniz.
<br><br><br>
{{% liman-image-viewer "politikalar-ve-eklentiler/liman-mys-dns-1.png" %}}
<br><br>
<hr>
{{% title4 "DNS Eklentisi" %}}
Linux ve Windows sistemlerinde bulunan DNS servislerini kolaylıkla yönetebilirsiniz. Eklentide alan oluşturma, alanlara kayıt ekleme, kayıtları düzenleme, kayıt silme gibi fonksiyonların tamamı kararlı şekilde yapılabilmektedir. 
<br><br><br>
{{% liman-catalog "create" "dns" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-dns-1.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-dns-2.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-dns-3.png" %}}
{{% liman-catalog "end" "dns" %}}
<br><hr>
{{% title4 "PXE Boot Eklentisi" %}}
PXE boot, bilgisayar üzerinde herhangi bir depolama alanına (Hard disk, CD-DVD vb.) ihtiyaç duymadan ağ  kartının yardımı ile bilgisayarın ilk açılışını sağlayan sistemdir. PXE ortamı, DHCP ve BOOTP protokollerini kullanarak ağa bağlanırken, TFTP protokolü yardımıyla da gerekli önyükleme programını yükleyerek işletim sisteminin açılmasını sağlar. Eklentimizde açılan işletim sistemine imaj alma, imaj yükleme, parça imaj alma ve parça imaj yükleme gibi işlemleri gerçekleştirebileceğiniz butonları kolaylıkla oluşturabilir ve yönetebilirsiniz. İmaj alırken veya yüklerken NFS sunucusu, harici disk veya SSH gibi seçenekler bulunmaktadır. Aldığınız imajları bir sunucuda tutuyor iseniz imaj isimleri, imaj boyutlarını görebileceksiniz. Sunucuya imaj yükleyip, kolaylıkla imaj silebileceksiniz. 
<br><br><br>
{{% liman-catalog "create" "pxe" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-pxe-1.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-pxe-2.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-pxe-3.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-pxe-4.png" %}}
{{% liman-catalog "end" "pxe" %}}
<br><hr>
{{% title4 "Repository Eklentisi" %}}
Ubuntu ve Debian depolarını kolaylıkla aynalayabilirsiniz. Bu sayede internete ihtiyaç olmadan paketlerinizi aynalanan depodan güncelleyebilirsiniz. Aynalanan depolarda paket araması yapabilirsiniz. Aynalama işlemlerinde kimin hangi depoyu aynaladığını görebilmenizi sağlayan loglar tutulmaktadır. Bunun haricinde yerel depo sekmesinde kendi deponuzu oluşturabilirsiniz. Bu depoya arayüzden istediğiniz paketleri ekleyip çıkartabilirsiniz. Dış depo sekmesinde ise istediğiniz depo adresini ekleyip aynalama yapmadan içindeki paketleri listeleyip görebilirsiniz.
<br><br><br>
{{% liman-catalog "create" "repo" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-repo-1.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-repo-2.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-repo-3.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-repo-4.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-repo-5.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-repo-6.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-repo-7.png" %}}
{{% liman-catalog "add" "politikalar-ve-eklentiler/liman-mys-repo-8.png" %}}
{{% liman-catalog "end" "repo" %}}
<br>