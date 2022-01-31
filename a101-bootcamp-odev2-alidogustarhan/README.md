# Ödev 2

##### 1-Proje ``` npm start ``` ile çalışıyor ve ilgili dosya konumuna cd yazarak JTW-main dosyasını sürükle bırak yaparak bu dosyanın konumuna geçiniz.

##### 2-Projenin çalışması için terminale npm init yazarak node_modules klasörürün indirme işlemini yapınız.

##### 3-Projede gözüken .env dosyası token olustururken ek güvenlik olarak bir parametre olması amacıyla kullanılmıştır.Normalde bu dosya .gitignore içerisine atılır. Ancak bu    projede açık olarak yolladık.

##### 4-Projemizde token oluştururken kullandığımız id parametresinin normalde DataBase den çekilmesi gerekmektedir.Ancak bu projemizde DB entegre olmadığı için random metodu ile bu sayıyı ürettik.

##### 5-Projemiz frontend kısmına entegre edilmiştir. Projenin çalışması için npm start ile projeyi çalıştırdıktan sonra tarayıcınızdan locahost:3000 adresine gitmeniz yeterlidir.

##### 6-Projemizde api den data çekebilmeniz için öncelikle login olmanız gerekmektedir. Login işlemi için username:ADMIN password:1234 yazmanız gerekmektedir. Aksi halde giriş yapamazsınız.

##### 7-Frontend kısmında çalışırken login yaparak ürettiğiniz token Local Storage ye kaydolur. Dolayısıyla uygulamayı yeniden denemek için f12 ye basıp ilgili Local Storage yi silmeniz gerekmektedir. Aksi taktirde data çekme işlemi sürekli aktif olacaktır.Ayrıca frontend kısmıda çektiğimiz datalar Object şeklinde gözükmektedir.Dataları daha detaylı görmek için uygulamayı postman de kullanınız.

##### 8-Uygulamayı postmande kullanırken login olmak için localhost:3000/api/v1/login yolunu kullanınız.(POST) Burada size verdiğim username ve password u ilgili adresi kullanarak JSON formatında POST ediniz.

##### 9-Login işleminden sonra gelen token i kopyalayınız. Trendyol dan tüm markaları çekmek için  localhost:3000/api/v1/dashboard yolunu , trendyoldan istediğiniz markayı çekmek için localhost:3000/api/v1/dashboard/VERSACE örnek yolunu ve benzer şekilde diğer kategoriler için de kodda belirtilen api yollarını kullanabilirsiniz. Get ile yollamanız gerekmektedir. Dilediğiniz markayı VERSACE yazan yere yazarak ilgili data yı elde edebilirsiniz. 

##### 10-Postmande çalışırken uygulamayı yeniden denemek isterseniz yine ilgili Token'ı silmeyi unutmayınız.




### Node.JS
JavaScript kullanarak sunucu tarafında çalışan uygulamalar geliştirebileceğimiz bir Back-End teknolojisidir. JavaScript temelli olmasından dolayı dinamik ve hızlı bir yapısı vardır. En önemli özelliği ise asenkron yapıda çalışmasıdır. 

### Joi
JavaScript için şema hazırlayarak veri doğrulamayı sağlayan bir npm kütüphanesidir. 
JSON Web Token (JWT), iletişim yapan birimler arasındaki veri alışverişinin güvenli bir şekilde sağlanması için bir JSON nesnesi (token) kullanarak daha kompakt ve bilginin kendini kendini betimlediği bir yol sunan endüstri standardıdır.

### JWT

JSON Web Token (JWT), veri alışverişinin güvenli bir şekilde sağlanması için JSON nesnesi (token) kullanarak bilginin kendini kendini betimlediği bir yol sunan standarttır. 

JWT kullanabileceğimiz zamanlar: 

###### Kimliklendirme: 
En temel kullanım senaryosu olduğu söylenebilir. Kullanıcının başarılı giriş işlemi sonrasında gerçekleştireceği her istek JWT’yi içermektedir. Böylelikle kullanıcının ulaşacağı kaynaklara/web sayfalarına erişim bilgisi bu token bilgisi ile kontrol edilebilmektedir. Farklı domainler arasında kolayca token değiş-tokuşu sağlandığı için, tek seferlik giriş (single sign on) senaryolarında yoğun olarak kullanılabilmektedir.

###### Bilgi değiş-tokuşu: 
JWT’ler dijital olarak imzalanabilmektedir. Bu yüzden de bilginin iletişim yapan birimler arası güvenli bir şekilde gerçekleşebilmesi için iyi bir yöntem sunmaktadır. Örneğin açık/gizli anahtar ikilileri kullanıldığında bilgiyi gönderen kişinin gerçekte kim olduğunu söylemek mümkün olmaktadır. Buna ek olarak ise JWT’deki header ve payload kısımları dahil edilerek oluşturulan imza sayesinde gelen bilginin değiştirilip/değiştirilmediği kolayca doğrulanabilmektedir.



