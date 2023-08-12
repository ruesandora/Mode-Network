<h1 align="center"> Mode Network </h1>

> Başlangıçta `köprüyü` kullanalım ve biraz Mode ağında test tokenımız olsun.

> [Buradan](https://bridge.mode.network/) kullanabilirsiniz köprüyü. Ben Mode Network'u `çok sevdim çok.`

```
# RPC bilgileri:
Mode Testnet
https://sepolia.mode.network
919
mETH
```

> Öncelikle [Buradan](https://thirdweb.com/dashboard/settings/api-keys) `create API keys` diyip bilgilerimizi kaydediyoruz.

> Sonra buradan gerekli komutlarımızı girelim:

```
sudo apt update
sudo apt upgrade

# npm'i indiriyoruz:
sudo apt install nodejs

# thirdwebî indiriyoruz:
npm i -g thirdweb

# token oluşturmak için:
npx thirdweb create
# bu komuttan sonra görselde ki değerleri seçebilir veya girebiliriz:
```

![image](https://github.com/ruesandora/Mode-Network/assets/101149671/0be295d1-3e9c-428e-81a4-a4203b42df63)

> Artık kendimize ait mode zincirinde token var ben Thridweb'i çok seviyorum neredeyse tüm evm zincirlerinde bunu yapabilirsiniz.

> şimdi bu komutu girelim ve kontratımızı deploy edelim.

```
npx thirdweb deploy
> bu komut sonrası çıktıya API keylerimizden secrey key'i girelim.
> Akabinde bize çıktı olarak bir link verecek onu google'da açalım. Ve cüzdan bağladıktan sonra deploy now diyelim.
> Token ismi, token kısaltması ve cüzdan adresimizi girelim ve deploy diyelim Mode ağında.
> Artk tokeniniz var, bu token ile thridweb'de bir çok şey yapabilirsiniz bundan sonrasını size bırakıyorum.
> Ben anlatırsam her şeyi anlamı kalmaz kurcalayın, token supply arttırın, airdrop yapın trnasfer yapın.
```

> Yaptığınız işlemleri de bu repo'ya klasor olarak `PR` yapın öğrenin iyice, hatta bana da token atın.

> Adresim: `0x941bCb9Fda08f085ebCf36E4e11e5cf245Db00C6`

> ayrıca OG rolü almak için galxe falan var ama ben onları bılmıyorum siz bakarsınız. Bu konuda rehber yazarsanız bu repoya PR atarsınız.


<h1 align="center"> unexpected token hatası alanlar için </h1>

```
# kaldıralım
sudo apt remove nodejs npm

# Yeniden yükleyelim:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash

source ~/.bashrc
nvm install node
```

> daha sonra thirdwebi indiriyoruz adımından devam edebilirsiniz.

> Ayrıca deploy hatası alanlar için cd ile oluşturduğunuz proje ismindeki klasöre girip deploy komutunu çalıştırın
