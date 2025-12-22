# PHP Hello World - Coolify Auto Deploy

Basit bir PHP uygulaması. GitHub üzerinden Coolify'a otomatik deploy için hazırlanmıştır.

## Özellikler

- Basit "Hello World" PHP uygulaması
- Modern ve responsive tasarım
- PHP versiyonu ve tarih bilgisi gösterimi

## Coolify Kurulum Adımları

### 1. GitHub Repository Oluşturma

1. Bu projeyi GitHub'a push edin:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/KULLANICI_ADI/REPO_ADI.git
   git push -u origin main
   ```

### 2. Coolify'da GitHub App Oluşturma

1. Coolify kontrol panelinde **"Sources"** sekmesine gidin
2. **"New Source"** butonuna tıklayın
3. **"GitHub App"** seçeneğini seçin
4. GitHub'da yönlendirileceksiniz, burada:
   - Uygulama adını girin
   - Gerekli izinleri verin (repository access)
   - Uygulamayı oluşturun

### 3. Coolify'da Uygulama Oluşturma

1. Coolify ana sayfasında **"New Resource"** butonuna tıklayın
2. **"Application"** seçeneğini seçin
3. **"Private Repository (with GitHub App)"** seçeneğini seçin
4. Oluşturduğunuz GitHub App'i seçin
5. GitHub repository'nizi seçin ve yükleyin
6. Uygulama ayarlarını yapılandırın:
   - **Build Pack**: PHP (otomatik algılanır)
   - **Port**: 80 (veya istediğiniz port)
   - **Domain**: Uygulamanız için domain adı

### 4. Auto Deploy Aktifleştirme

1. Oluşturduğunuz uygulamanın ayarlarına gidin
2. **"Advanced"** sekmesine tıklayın
3. **"Auto Deploy"** seçeneğini aktifleştirin
4. Değişiklikleri kaydedin

### 5. İlk Deploy

1. Uygulama sayfasında **"Deploy"** butonuna tıklayın
2. Coolify otomatik olarak:
   - Repository'yi clone edecek
   - PHP uygulamanızı build edecek
   - Container'ı başlatacak

## Otomatik Deploy

Auto Deploy aktif olduktan sonra:
- GitHub repository'nize her push yaptığınızda
- Coolify otomatik olarak değişiklikleri algılayacak
- Uygulamanızı otomatik olarak yeniden deploy edecek

## Manuel Deploy

Eğer otomatik deploy istemiyorsanız:
- Coolify uygulama sayfasında **"Deploy"** butonuna tıklayarak manuel deploy yapabilirsiniz

## Notlar

- Coolify otomatik olarak PHP uygulamalarını algılar
- Özel Dockerfile gerekmez (Coolify otomatik oluşturur)
- PHP versiyonu Coolify'ın varsayılan PHP image'ına bağlıdır
- İhtiyaç duyarsanız `Dockerfile` veya `coolify.yaml` dosyası ekleyebilirsiniz

## Destek

Sorun yaşarsanız:
- [Coolify Dokümantasyonu](https://next.coolify.io/docs)
- [Coolify GitHub](https://github.com/coollabsio/coolify)

