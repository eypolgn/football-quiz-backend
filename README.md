# Football Quiz App

Football Quiz App, kullanıcıların futbol bilgilerini test edebileceği bir web uygulamasıdır. Kullanıcılar, bir zorluk seviyesi seçip rastgele seçilmiş soruları cevaplayabilirler. Uygulama, kullanıcı puanlarını takip eder ve liderlik tablosunda gösterir.

## Özellikler

- **Soru Yönetimi**: Futbol bilgi yarışması soruları ekleyebilir ve sorgulayabilirsiniz.
- **Liderlik Tablosu**: Kullanıcı puanlarını takip eder ve zorluk seviyesine göre sıralar.
- **Zorluk Seviyeleri**: Kullanıcılar farklı zorluk seviyeleri arasından seçim yapabilir.
- **CORS Yapılandırması**: Frontend'den gelen farklı bir orijinden gelen isteklere izin verir.

## Teknolojiler
- **Backend**: Java, Spring Boot
- **Veritabanı**: PostgreSQL
- **Bağımlılıklar**:
  - Spring Web
  - Spring Data JPA
  - Lombok
  - Jakarta Persistence API

## Proje Yapısı

- **Controller**: Gelen HTTP isteklerini işler ve uygun servis yöntemlerine yönlendirir.
  - `QuestionController`: Bilgi yarışması sorularını yönetir.
  - `LeaderboardController`: Liderlik tablosu girişlerini yönetir.
- **Service**: Uygulamanın iş mantığını içerir.
  - `QuestionService`: Soru ile ilgili işlemleri gerçekleştirir.
  - `LeaderboardService`: Liderlik tablosu ile ilgili işlemleri gerçekleştirir.
- **Model**: Uygulamada kullanılan veri yapısını temsil eder.
  - `Question`: Seçenekleri ve doğru cevabı ile bir bilgi yarışması sorusunu temsil eder.
  - `LeaderboardEntry`: Liderlik tablosundaki bir girişi temsil eder.
- **Repository**: Veritabanı işlemleri için arayüzler.
  - `QuestionRepository`: `Question` entity'leri için CRUD işlemleri.
  - `LeaderboardRepository`: `LeaderboardEntry` entity'leri için CRUD işlemleri.

## Kurulum

1. **Repository'yi klonlayın**:
   ```bash
   git clone https://github.com/your-username/FootballQuizApp.git
   cd FootballQuizApp
