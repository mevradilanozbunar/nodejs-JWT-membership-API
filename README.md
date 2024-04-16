# Node.js JWT ile Üyelik Sistemi API

Bu proje, Node.js kullanılarak geliştirilmiş bir üyelik sistemi API'si sağlar. JSON Web Token (JWT) kullanılarak kimlik doğrulama ve yetkilendirme sağlanır. Kullanıcı kaydı, girişi, profil bilgilerinin alınması, şifre sıfırlama gibi işlemleri gerçekleştirebilirsiniz.

## Kullanılan Teknolojiler

- Node.js
- Express.js
- MongoDB
- JWT (JSON Web Token) ile kimlik doğrulama
- bcrypt ile şifreleme
- Joi ile veri doğrulama
- Nodemailer ile e-posta gönderme
- express-rate-limit ile API isteklerinin sınırlanması
- express-mongo-sanitize ile MongoDB sorgularının güvenli hale getirilmesi
- cors ile Cross-Origin Resource Sharing (CORS) yönetimi

## Başlarken

1. Projeyi klonlayın:
 
   ```sh
   git clone https://github.com/mevradilanozbunar/nodejs-JWT-membership-API.git
   ``` 
3. Proje dizinine gidin:
 
    ```sh
   cd nodejs-JWT-membership-API
   ``` 
5. Gerekli bağımlılıkları yükleyin:
 
    ```sh
   npm install
   ``` 
7. `.env` dosyasını oluşturun ve gerekli ortam değişkenlerini ayarlayın (örneğin, veritabanı bağlantısı, JWT anahtarı, e-posta hesabı vb.).
   
8. Uygulamayı başlatın:
   
    ```sh
   npm start
   ``` 

## Endpoints

- `POST /api/login`: Kullanıcı girişi için
- `POST /api/register`: Kullanıcı kaydı için
- `GET /api/me`: Mevcut kullanıcı bilgilerini getirir
- `GET /api/users`: Tüm kullanıcıları getirir (Yönetici için)
- `POST /api/forget-password`: Şifreyi sıfırlamak için sıfırlama kodu oluşturur ve e-posta gönderir
- `POST /api/reset-code-check`: Sıfırlama kodunun doğruluğunu kontrol eder
- `POST /api/reset-password`: Şifreyi sıfırlar
 
