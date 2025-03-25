
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
```bash
gemini-cli :code example.py "Kullanıcıya IP adresini yazdırtan bir python kodu yaz"
gemini-cli :img eyfel_kulesi.png "Bana eyfel kulesini gerçekçi şekilde çiz"
gemini-cli :help "sudo dpkg -i package.deb"
gemini-cli :sh "Nasıl Masaüstü dizinindeki tüm txt dosyalarını bulurum?"
```
