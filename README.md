<h1 align="center"> Mode Network </h1>

> Başlangıçta `köprüyü` kullanalım ve biraz Mode ağında test tokenimiz olsun.

> [Buradan](https://bridge.mode.network/) kullanabilirsiniz köprüyü. Ben Mode Network'u `çok sevdim çok.`

```
# RPC bilgileri:
Mode Testnet
https://sepolia.mode.network
919
mETH
```

> Öncelikle [Buradan](https://thirdweb.com/dashboard/settings/api-keys) `create API keys` diyip istediğimiz bir isim veriyoruz ve next diyoruz.
Çıkan ekranda secret keyi kaydediyoruz. Daha sonra lazım olacak.


> Sonrasında [Buradan](https://github.com/codespaces)
> "Use This Templete" diyerek terminalin gelmesini bekleyelim.
![image](https://github.com/AbdullahCoban28/Mode-Network/assets/111288151/9dbf6e75-e012-4922-bc0f-a90410b24834)

> Terminal geldikten sonra buradan gerekli komutlarımızı girelim:

```
sudo apt update
sudo apt upgrade

# npm'i indiriyoruz:
sudo apt install nodejs

# thirdwebî indiriyoruz:
npm i -g thirdweb

# token oluşturmak için:
npx thirdweb create
# bu komuttan sonra görseldeki değerleri seçebilir veya girebiliriz:
```

![image](https://github.com/ruesandora/Mode-Network/assets/101149671/0be295d1-3e9c-428e-81a4-a4203b42df63)

> Artık kendimize ait mode zincirinde token var ben Thirdweb'i çok seviyorum neredeyse tüm evm zincirlerinde bunu yapabilirsiniz.

> Şimdi bu komutu girelim ve kontratımızı deploy edelim.
```
npx thirdweb deploy --key <thirdwebden aldığınız secret key>
```
Bunu yazdığınızda tokeniniz başarılı bir şekilde oluşturulacaktır ve sizi thirdweb sitesine yönlendirecektir.

>Contracts Kısmından Deploy contract diyoruz

![image](https://github.com/AbdullahCoban28/Mode-Network/assets/111288151/f6e62762-1c38-4f8a-af50-13bd0269c0e2)

>Karşımıza yapabileceğimiz bir çok şeyi sunan bir sayfa açılıyor.Ben burada 5.sıradaki yere tıklayarak token oluşturmaya geçtim.

![image](https://github.com/AbdullahCoban28/Mode-Network/assets/111288151/cff2c59c-3d15-4b3a-bfa9-e0d47b81fcd6)

>Burada aşağıda code olarak eklemeler çıkarmalar yapılabilir fakat ben yapmadım. Deploy Now diyoruz.

![image](https://github.com/AbdullahCoban28/Mode-Network/assets/111288151/3b7a97a8-d714-4537-a4d3-e8ee808ac903)

> Deploy Now dediğimizde bizden bilgiler isteyecek.Tokenimizin adı sembolü resmi bunları seçtikten sonra en önemli kısım en altta bulunan network chain kısmında 
MODE NETWORK seçtiğimizden emin olalım ve en baştaki bridge den eth atmış olalım.

![image](https://github.com/AbdullahCoban28/Mode-Network/assets/111288151/0e30ae9a-db9c-4988-9cb3-4e390ddfd1ca)

>Tokenimiz artık oluştu ve contracts kısmına geldiğimizde sağdaki seçeneklerden tokene tıkladığımızda

>Burn, airrop,transfer ve mint yapabiliriz. İstediğimiz kadar token mitleyebilir ve transfer edebiliriz.

![image](https://github.com/AbdullahCoban28/Mode-Network/assets/111288151/6964fd05-dcce-4d13-8461-d3de8c064217)

> Yaptığınız işlemleri de bu repo'ya klasör olarak `PR` yapın öğrenin iyice, hatta bana da token atın.

> Adresim: `0x941bCb9Fda08f085ebCf36E4e11e5cf245Db00C6`

> Ayrıca OG rolü almak için galxe falan var ama ben onları bilmiyorum siz bakarsınız. Bu konuda galxe linkini bırakıyorum siz inceleyebilirsiniz.
> 
> Mode Network Galxe https://galxe.com/mode şuan aktif etkinlik yok yakın zamanda başlar büyük ihtimalle.

```
<h1 align="center"> unexpected token hatası alanlar için </h1>

# kaldıralım
sudo apt remove nodejs npm

# Yeniden yükleyelim:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash

source ~/.bashrc
nvm install node
```

> daha sonra thirdwebi indiriyoruz adımından devam edebilirsiniz.

> Ayrıca deploy hatası alanlar için cd ile oluşturduğunuz proje ismindeki klasöre girip deploy komutunu çalıştırın.
