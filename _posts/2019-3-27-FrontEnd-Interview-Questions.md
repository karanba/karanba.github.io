---
layout: post
title: Front-End İş Görüşmesi Soruları 
--- 


## Front-End İş Görüşmesi Soruları?

###HTML

#### HTML Nedir? Temel Karakteristik özellikleri nedir? 

HTML - HyperText Transfer Protocol olarak kısaltılmış bir iletişim protokolüdür? İstemci ve Sunucu mimarisi üzerine kurulmuştur. Uygulama katmanında bulunur. En yaygın kullanılan versiyonu HTTP 1.1 dir. 

Temelde istemcinin bir istek - request - ile iletişimi başlatması ile açılna bağlantı üzerinden sunucunun cevap - response - vermesi şeklinde gerçeklşir. İstekte protokol ve versiyon bilgileri ile beraber erişilmek istenen host ve path bilgileri geçilir. Path bilginin yanı sıra QueryString tabir edilen URL parametreleride geçilebilir. Bunun yanı sıra istek başlık bilgileri - request header-, isteğin gövde kısmıda  - body - istek ile birlikte gönderilir. Karşılığında alınan cevapta, , durum kodu - status code -, cevap uzuluğu, durum kod metni - status mesaj -, başlık bilgileri - response header - ve duruma göre cevap gövdesi - response body - bulunur.

#### HTTP Protokolü - Stateless - olarak tanımlanması neyi ifade eder? Stateless ve Stateful kavramlarını açıklayabilir misiniz?

Stateless kavramı, yapılan istekler arasından HTTP açısından bir ilişki olmamasını ve her isteğin bir birine bağlı olmadan gönderilmesi manası taşır. HTTP stateless bir protocol olması, sessionless olduğu manasına gelmez. Stateless bir başka ifade ile state bilgisinin nerede saklandığı ile ilişkilidir. Eğer istemci state bilgisini tutuyorsa protocol stateless denir, eğer sunucu state bilgisini tutuyorsa protocol stateful tabir edilir. Mesela TCP taşıma katmanında stateful protokol örneğidir. Uygulama katmanındada FTP stateful bir protokoldur. Stateful protokoller istemciyi dump olarak kabul ederler. Buna karşın stateless protokollerde istemci akıllı - smart - olarak kabul edilirer. Gün sonunda altaki protokol stateless olsada biz uygulamalarımızda state bilgisine ihtiyaç duyarız. Bunun içinde state bilgisini saklamak ve taşımak üzere çeşitli yöntemler geliştirilmiştir. 
