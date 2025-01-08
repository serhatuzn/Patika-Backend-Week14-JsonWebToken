# JWT Projesi 🔐

**JWT (JSON Web Token)** Projesine hoş geldiniz! Bu depo, ASP.NET kullanılarak güvenli kimlik doğrulama ve yetkilendirme için bir JWT uygulaması içermektedir. Aşağıda projenin genel bir bakışını, nasıl kurulacağını ve etkili bir şekilde nasıl kullanılacağını bulabilirsiniz.

## Özellikler ✨
- **Güvenli Kimlik Doğrulama**: Token tabanlı kimlik doğrulama için JWT uygular.
- **Token Doğrulama**: Token'ların bütünlüğünü ve geçerliliğini sağlar.
- **Yapılandırılabilir Süre Sonu**: Güvenliği artırmak için token'lar için bir sona erme mekanizması.
- **ASP.NET Backend**: Modern ASP.NET uygulamaları ile geliştirilmiştir.

## Proje Yapısı 🌐
```
JWT_extracted/
|
|-- src/                         # Kaynak kod dizini
|    |-- main/                   # Ana uygulama kodları
|        |-- aspnet/             # JWT mantığı için ASP.NET dosyaları
|        |-- resources/          # Yapılandırma dosyaları (ör. appsettings.json)
|
|-- README.md                    # Proje dokümantasyonu
|-- logs/                        # Log dosyaları
|
|-- test/                        # Birim test dosyaları
```

## Gereksinimler ⚡
- **.NET SDK**: .NET Core veya .NET 5/6 versiyonu.

## Kurulum ve Yükleme 🔧
1. **Depoyu Klonlayın**:
   ```bash
   git clone <repository-url>
   ```
2. **Proje Dizinine Geçin**:
   ```bash
   cd JWT_extracted
   ```
3. **Bağımlılıkları Yükleyin**:
   ```bash
   dotnet restore
   ```
4. **Uygulamayı Çalıştırın**:
   ```bash
   dotnet run
   ```

## Kullanım 🌎
1. **Token Oluşturun**:
   - Geçerli kullanıcı bilgileriyle `/generate-token` endpoint'ine bir POST isteği gönderin.
2. **Token Doğrulayın**:
   - `/validate-token` endpoint'ini kullanarak bir token'ın geçerliliğini doğrulayın.
3. **Güvenli Endpoint'ler**:
   - `Authorization` başlığına token'ı ekleyerek güvenli endpoint'lere erişin.

## Yapılandırma 🔧
- `appsettings.json` dosyasını düzenleyerek gizli anahtar, token süresi gibi ayarları güncelleyin.

Örnek:
```json
{
  "Jwt": {
    "Secret": "your-secret-key",
    "ExpiryInMinutes": 60
  }
}
```

## Testler ✅
- Birim testleri çalıştırmak için:
  ```bash
  dotnet test
  ```

## Loglar 🔍
- Uygulama logları `logs/` dizininde saklanır. Hata ayıklama veya izleme için bu dosyaları kontrol edin.

## Katkıda Bulunun ❤
Katkılara açığız! Bu projeyi geliştirmek için sorun veya pull request göndermekten çekinmeyin.

## Lisans 🔒
Bu proje MIT Lisansı ile lisanslanmıştır. Detaylar için `LICENSE` dosyasına bakabilirsiniz.

---

İyi kodlamalar! 🚀 Herhangi bir sorunuz olursa, bize ulaşmaktan çekinmeyin. 🙌
