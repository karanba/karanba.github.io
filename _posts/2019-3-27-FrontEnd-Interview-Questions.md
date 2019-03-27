---
layout: post
title: Front-End İş Görüşmesi Soruları 
categories: [Front-End]
tags: [http, html, css, javascript, interview]
level: Başlangıç
lang: tr
blog: yes
--- 

Front-End iş görüşmlerinde yararlı bir kaynak olması umudu ile teknik görüşmede sorulabilecek bazı soruları ve cevaplarını yazmaya çalıştım. Umarım faydalı olur.

## Front-End İş Görüşmesi Soruları?

### HTTP

#### HTTP Nedir? Temel Karakteristik özellikleri nelerdir? 

HTTP - HyperText Transfer Protocol - bir iletişim protokolüdür? İstemci ve Sunucu mimarisi üzerine kurulmuştur. Uygulama katmanında yer alır. En yaygın kullanılan versiyonu HTTP 1.1 dir. 

Temelde istemcinin bir istek - request - ile iletişimi başlatması ile açılna bağlantı üzerinden sunucunun cevap - response - vermesi şeklinde gerçeklşir. İstekte protokol ve versiyon bilgileri ile beraber erişilmek istenen host ve path bilgileri geçilir. Path bilginin yanı sıra QueryString tabir edilen URL parametreleride geçilebilir. Bunun yanı sıra istek başlık bilgileri - request header-, isteğin gövde kısmıda  - body - istek ile birlikte gönderilir. Karşılığında alınan cevapta, , durum kodu - status code -, cevap uzuluğu, durum kod metni - status mesaj -, başlık bilgileri - response header - ve duruma göre cevap gövdesi - response body - bulunur.

#### HTTP Protokolü - Stateless - olarak tanımlanması neyi ifade eder? Stateless ve Stateful kavramlarını açıklayabilir misiniz?

Stateless kavramı, yapılan istekler arasında  bir ilişki olmamasını ve her isteğin bir birine bağlı olmadan gönderilmesi manası taşır. HTTP stateless bir protocol olması, sessionless olduğu manasına gelmez. Stateless bir başka ifade ile state bilgisinin nerede saklandığı ile ilişkilidir. Eğer istemci state bilgisini tutuyorsa, protocol stateless olarak ifade edilir. Eğer sunucu state bilgisini tutuyorsa, protocol stateful olarak tabir edilir. Mesela TCP taşıma katmanında stateful bir protokol örneğidir. Uygulama katmanında ise FTP stateful bir protokol örneğidir. REST mimarisinde hazırlanan servisler stateless servislere örnek verilebilir. İlişkisel veritabanı yönetim bağlantıları ise sateteful olarak çalışır. Stateful protokoller istemciyi boş - dump - olarak kabul ederler. Buna karşın stateless protokollerde istemci akıllı - smart - olarak kabul ederler. Gün sonunda altaki protokol stateless olsada biz uygulamalarımızda state bilgisine ihtiyaç duyarız. Bunun içinde state bilgisini saklamak ve taşımak üzere çeşitli yöntemler geliştirilmiştir. 

Eğer bahsi geçen protokolün veya servisin stateful mu yoksa stateless mı olduğunu kavramada zorluk çekiliyor  ise şu kritere göre değerlendirme yapılabilir. İstekleri bir vekil -proxy- sunucu üzerinden farklı sunuculara gönderdiğinizde herhangi bir aksama olmuyorsa bu durumda stateless çalışıyorsunuz demektir. Burada ki vekil basit şekilde herhangi bir katkı oluşturmadan gelen istekleri rast gele arkadaki sunuculara dağıtıldığını varsayıyoruz. 

Stateless bir iletişimde, gereken tüm bilgiler her isteğin içinde bulunmak durumundadır. Mesela kullanıcıyı tanımaya yönelik bir session id veya token her seferinde geçilmelidir. Buna karşın stateless durumda bağlantı süreli olarak açık bırakılmak zorunda kalmaz ve kullanıc takibi yapılmaz. Yük dengeleme için uygundur.
 

#### Bir Web Aplikasyonunda nasıl session oluşturulabilir?
...

### HTTP Caching nasıl yapılır?

HTTP caching temelde cache-control başlık bilgisi üzerinden yönetilebilir. Bunun yanında HTTP 1.0 a özgü _pragma_ başlık bilgisi bulunmaktadır. Cache-control yanında Etag, Expires, Last-Modified başlık bilgileride cache validasyonu için kullanılırlar 

#### no-cache ve no-store arasında ne fark vardır?
...

#### Private ve Public cache nedir?
...

#### Etag ve Expires kullanımını kıyaslayınız? 
...



### HTML

#### HTML Nedir? Temel elementler nelerdir

#### Sayfada link vermek için hangi tag kullanılabilir?

##### Tıklanan linklerin yeni pencerede veya tab da açılması nasıl sağlanır?

##### Div ve Span arasındaki farklar nedir?

### CSS

#### CSS Nedir? CSS sayfaya nasıl eklenir?
...

#### Display özelliği hangi degğerleri alır ve arasındaki farklar nelerdir?
...

#### Position özelliği hangi degğerleri alır ve arasındaki farklar nelerdir?
...



