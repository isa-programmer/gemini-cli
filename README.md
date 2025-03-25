# gemini-cli

Terminalinizde kullanabileceğiniz yapay zeka

## Kurulum
```bash
git clone https://github.com/isa-programmer/gemini-cli
cd gemini-cli
pip install -r requirements.txt
chmod +x gemini-cli
sudo cp gemini-cli /usr/local/bin/
```

## API Anahtarı ekleme
```bash
echo GEMINI_API_KEY=XXXXXXXXXXX >> ~/.gemini.env # XXX yazan yere kendi API anahtarınızı ekleyin ve anahtarı kimse ile paylaşmayın
```

## Kullanmaya başlama

### Kod Oluşturma
```bash
gemini-cli :kod example.py "Kullanıcıya IP adresini yazdırtan bir python kodu yaz"
```

### Görsel Oluşturma
```bash
gemini-cli :resim eyfel_kulesi.png "Bana eyfel kulesini gerçekçi şekilde çiz"
```

### Görsel Analizi
```bash
gemini-cli :analiz resim.jpg
```

### Dosya Hakkında Soru Sorma
```bash
gemini-cli :soru dosya.txt "Bu dosya ne hakkında ve içinde hangi bilgiler var?"
```

### Hava Durumu Sorgulama
```bash
gemini-cli :hava "İstanbul"
```

### Döviz Kurlarını Sorgulama
```bash
gemini-cli :kur TRY    # TRY bazında kurları gösterir
gemini-cli :kur USD    # USD bazında kurları gösterir
```

### Bash Komutu Yardımı
```bash
gemini-cli :help "sudo dpkg -i package.deb"
```

### Bash Komutu Oluşturma
```bash
gemini-cli :sh "Nasıl Masaüstü dizinindeki tüm txt dosyalarını bulurum?"
```

### Yeni Özellikler

#### Sohbet Modu
Gemini ile interaktif olarak sohbet edebilirsiniz:
```bash
gemini-cli :sohbet
```

Sohbet sırasında aşağıdaki komutları kullanabilirsiniz:
- `exit`, `quit`, `çıkış`, `q`, `x`, `kapat`, `çık`, `son` - Sohbeti sonlandırmak için
- `:kaydet dosya.txt` - Sohbeti bir dosyaya kaydetmek için

#### Metin Özetleme
Uzun metinleri kısa ve öz bir şekilde özetleyebilirsiniz:
```bash
gemini-cli :özet "Özetlenmesini istediğiniz metin buraya yazılır..."
```

#### Metin Çevirme
Metinleri farklı dillere çevirebilirsiniz:
```bash
gemini-cli :çevir "Hello, how are you?" Türkçe İngilizce
# İlk parametre: çevrilecek metin
# İkinci parametre: hedef dil (çevrileceği dil)
# Üçüncü parametre (opsiyonel): kaynak dil (belirtilmezse otomatik tespit edilir)
```

## Özellikler

- [x] Kod oluşturma - `:code` komutu ile kod oluşturabilirsiniz
- [x] Görsel oluşturma - `:img` komutu ile görsel oluşturabilirsiniz
- [x] Görsel analizi - `:analiz` komutu ile görselleri analiz edebilirsiniz
- [x] Dosya hakkında soru - `:soru` komutu ile dosya hakkında sorular sorabilirsiniz
- [x] Hava durumu - `:hava` komutu ile hava durumu bilgisi alabilirsiniz
- [x] Döviz kurları - `:kur` komutu ile güncel döviz kurlarını görebilirsiniz
- [x] Bash komutları hakkında yardım - `:help` komutu ile bash komutları hakkında bilgi alabilirsiniz
- [x] Bash komutu oluşturma - `:sh` komutu ile bash komutu oluşturabilirsiniz
- [x] Sohbet modu - `:sohbet` komutu ile Gemini AI ile sohbet edebilirsiniz
- [x] Sohbet kaydetme - `:kaydet` komutu ile sohbetlerinizi kaydedebilirsiniz
- [x] Metin özetleme - `:özet` komutu ile metinleri özetleyebilirsiniz
- [x] Çeviri desteği - `:çevir` komutu ile metinleri farklı dillere çevirebilirsiniz
- [ ] Çoklu dil desteği (Arayüz için)

## Katkıda Bulunma

Katkıda bulunmak için:

1. Bu repo'yu fork edin
2. Yeni bir branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Değişikliklerinizi commit edin (`git commit -m 'Harika bir özellik ekle'`)
4. Branch'inizi push edin (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun
