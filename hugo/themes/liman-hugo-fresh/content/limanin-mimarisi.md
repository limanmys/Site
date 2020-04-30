---
page_title: Liman'ın Mimarisi
title: Liman'ın Mimarisi
include_footer: true
---

<style type="text/css">
	hr.rounded {
  border-top: 4px solid #eee;
  border-radius: 6px;
  margin-top: 50px;
  margin-bottom: 50px;
}
</style>

<!--{{% title3 "§1 Lorem" %}}-->
Liman Merkezi Yönetim Sistemi adından anlaşılacağı üzere sunucuları, istemcileri ve kullanıcıları uzaktan merkezi olarak mevcut dizin yapınızdaki Grup Politika Objeleri (GPO) ve geliştirdiğimiz politikalar ile yönetmenizi sağlar.
    
<br>

{{% liman-image-viewer "liman-mys-yapisi-sema.png" "is-three-quarters" %}}

<br>
Liman MYS ile kullanımda olan dizinlerin (Samba, Aktif Dizin) entegrasyonu hizmetler kesintiye uğramadan sağlanmaktadır. Liman MYS'nin bileşenleri: <a href="#anchor-liman"><b>Liman</b></a>, <a href="#anchor-kaptan"><b>Kaptan</b></a>, <a href="#anchor-tayfa"><b>Tayfa</b></a> olarak üçe ayrılmıştır. Bu bileşenler, Liman MYS'nin kararlı ve güvenli olarak çalışmasını sağlar.

<a id="anchor-liman"></a>
<hr class="rounded">

{{% liman-title-image "4" "Liman" "logos/liman_logo_base-outlined-icon.png" "30px" %}}
Liman, Kaptan sunucusunu yönetir. Grup Politika Objesi (GPO) oluşturma, silme, politika ekleme işlemleri Liman tarafından yapılır. Linux politikaları oluşturmak için Aktif dizin veya Samba Dizin üzerindeki politika objeleri kullanılır. Geliştirdiğimiz politikalar Grup Politikası Objeleri içerisine eklenir. Windows ve Linux politikaları farklı şekilde tanımlanır.

<a id="anchor-kaptan"></a>
<hr class="rounded">

{{% liman-title-image "4" "Kaptan" "steering-wheel.webp" "30px" %}}
İstemcileri yöneten, gerekli politikaları belirleyip istemcilere gönderen sunucudur.
<br><br>
<b>Kaptan‘ın görevleri aşağıda belirtilmiştir:</b>
<br>
• Aktif dizin, Samba gibi domain yöneticileri üzerinde organizasyon ünitelerini de göz önüne alarak sorgulama yapıp kullanıcı ve istemci politikalarını listeleme.<br>
• Aktif dizin, Samba gibi domain yöneticilerinden gerekeli politikaların güncellenip güncellenmediğini kontrol etme, politikaları yükleme.<br>
• İstemci ajanlarına politikaları gönderme.<br>
• İstemcilerden (Tayfa) politika loglarını toplama.<br>

<a id="anchor-tayfa"></a>
<hr class="rounded">

{{% liman-title-image "4" "Tayfa" "sailor.png" "30px" %}}
GNU/Linux istemcilerde kurulu politika ajanıdır. İstemci üzerinde kullanıcı ve makina politikalarını indirip uygulamakla yükümlüdür. 
<br><br>
<b>Tayfa’nın görevleri aşağıda belirtilmiştir:</b>
<br>
• Kaptan sunucusu üzerinden gerekli politikaları indirme.<br>
• Politikaların doğruluğunu kontrol etme.<br>
• Politikaları uygulama.<br>
• Politika sonuçlarını kontrol edip logları kaptan sunucusuna gönderme.<br>
• Tayfa eklentilerini Kaptan üzerinden sorgulamak ve indirmek.<br>
