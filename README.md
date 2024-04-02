# React-Markdown

## Nedir?

React Markdown, React uygulamalarında Markdown belgelerini kolayca görüntülemek için kullanılan bir kütüphanedir. Markdown, metin biçimlendirme ve yapısı için kullanılan hafif bir işaretleme dilidir.

## Kullanım Amacı

React Markdown, aşağıdakiler gibi durumlarda Markdown belgelerini görüntülemek için kullanılır:

 * Belgeler
 * Açıklamalar
 * Görev listeleri

Faydaları

  * Markdown şekilde hazırlanmış metini HTML'e çevirmek ve projelere uygun şekilde kullanmak için faydalıdır.
  * Kolay Entegrasyon: React uygulamalarına kolayca entegre edilebilir.
  * Canlı Ön İzleme: Belgeler değişiklik yapılırken gerçek zamanlı olarak önizlenebilir.
  * Esnek Özelleştirme: Özelleştirilmiş stiller ve bileşenler eklenerek Markdown belgeleri kişiselleştirilebilir.
  * Sıradan Markdown Desteği: Temel Markdown söz dizimini ve uzantılarını destekler.
  * Performans Optimizasyonu: Belgelerin büyük olması durumunda bile hızlı yükleme süreleri sağlar.

## Kullanım

React Markdown kullanmak için aşağıdaki adımları izleyin:

1. Kütüphaneyi yükleyin:

 ```bash
npm install react-markdown
```
 

2. Uygulamada kütüphaneyi içe aktarın:

 ```js
import ReactMarkdown from "react-markdown";
 ```

3. Markdown metnini bir değişkene atayın:

 ```javascript
const markdown =
Merhaba, Markdown! ;
```

4. Markdown metnini React Markdown bileşeninde görüntüleyin:

 ```javascript
<ReactMarkdown>{markdown}</ReactMarkdown>
 ```

Örnek Kod

Aşağıdaki örnek kod, bir Markdown belgesini React uygulamasında nasıl görüntüleyeceğinizi göstermektedir:

```javascript
import React, { useState } from "react";
import ReactMarkdown from "react-markdown";


const App = () => {
  const [markdown, setMarkdown] = useState("
  return (
    <div>
      <textarea value={markdown} onChange={(e) => setMarkdown(e.target.value)} />
      <ReactMarkdown>{markdown}</ReactMarkdown>
    </div>
  );
};

export default App;
```

Bu kod, metin alanına Markdown metni girildiğinde gerçek zamanlı olarak güncellenen bir markdown etiketlerini kullancıya uygun hale getirerek birer "HTML" öğelerine dönüştürür.
## Markdown kullanımı ile yapabileceklerimiz,

* Blog gönderileri ve web sayfaları için Markdown içeriği oluşturmak ve düzenlemek.
* Açık kaynak kodlu projeler için belgeler ve kullanıcı kılavuzları oluşturmak.
* Kişisel notlar ve görev listeleri için Markdown tabanlı not alma uygulamaları oluşturmak.
* API'ler tarafından gelen markdown metinleri html etiketlerine dönüştürerek projelermize entegre şekilde kullanmak.

Okuduğunuz için teşekkürler.
