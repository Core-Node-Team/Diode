# Diode

### 🔹 1. Genel sistem güncellemelerini yapalım
```
sudo apt update && sudo apt upgrade -y
```

### 🔹 2. Snap Paket Yöneticisi Kurulu mu Kontrol Et
(Genellikle Ubuntu’da yüklüdür, ama emin olalım)
```
sudo apt install snapd -y
```


### 🔹 3. Diode Node Paketini Kur
```
sudo snap install diode-node
```
Kurulumdan sonra diode-node arka planda çalışmaya başlar.



### 🔹 4. Düğüm Bilgilerini Kontrol Et
```
diode-node.info
```
Bu komut, düğümünüzün kimliği, bağlı olduğu ağ, çalışma durumu gibi bilgileri gösterir.

![image](https://github.com/user-attachments/assets/5880003f-19c9-42fc-88ce-493327a5e75a)


### 🔹 5. Diode İstemcisiyle Örnek Bir Web Yayını (İsteğe Bağlı)

Bir dizini Diode Ağı üzerinden yayınlamak istersen:
```
mkdir mysite
echo "Hello Diode" > mysite/index.html
diode publish mysite
```
Bu işlemden sonra sana özel bir *.diode.link URL’si oluşur. Web tarayıcında bu adresi ziyaret ederek içeriğini görebilirsin.


### 🔹 6. (İsteğe Bağlı) Düğüm Sürekli Çalışsın Diye Logları İzle
```
sudo snap logs diode-node -f
```
Bu komutla arka plandaki düğüm loglarını takip edebilirsin.

### 🔹 7.Platforma bağlanalım cüzdan bağlayalım

- https://diodenetwork.io/app/  adresine gidelim ve sıfır bir evm cüzdan olusturalım bağlıyalım. Bundan sonraki işlemlere masaüstünden devam.

### 🔹 8. Diode Collab masaüstü uygulamasını indirelim.

https://diode.io/joinzone/#close

- Sağ yukardan get app diyelim. uygun olanı indir kur ( kendi pcmiz yerine baska bir yere indirebilirisek daha iyi olur sonucta test ben uyarayım da)

![image](https://github.com/user-attachments/assets/625589b0-4a88-42de-a6dc-473c5ed415aa)



### 🔹 9. Kurduk açtık isim yazdık kaydolduk sonra aşağıdaki şekilde yeni zone bağlanmak için alttaki kodu yazıp join diyoruz. Burada sync uzun sürebilir dismiss diyip atlayalım.
```
p0xUHtufRS_tMNd9XRvnxbMmXPtOyRbPrQLnLN4j3VNsDhwSrpRYpwbnhMZ2
```

![joincode-entry-example](https://github.com/user-attachments/assets/0a61fb5e-af27-4f0b-9ddc-001c33b455b2)



### 🔹 10. Aşağıdaki katılım kodunu resimde görünen registrar kanalına atıyoruz. Bu kodu girdikten sonra kabul edip etmediğinizi soracak I Accept yazarak devam edebilirsiniz. Kabul ettikten sonra size özel bir katılım kodu verecek siz de o kodla başkalarını davet edebileceksiniz.
```
GJTCTZTFRAPNVNJXSXGE
```

![image](https://github.com/user-attachments/assets/52afa1d9-fc94-423b-89dd-64cab864e279)


### 🔹 11. Platforma bağladığımız cüzdan adresimizi alalım ve aşağıdaki şekilde resimdeki gibi bota yazarak cüzdanımızı kayıt edelim. Cüzdan kaydı bir kere yapmanız yeterlidir.
```
set wallet EVMCUZDANADRESINIZ
```
![image](https://github.com/user-attachments/assets/8b5d8329-a5ee-4693-8565-bc472552e34b)


### 🔹 13. Çalıştırdığımız nodumuzu aşağıdaki örnekte görüldüğü gibi kayıt edelim. NODEID yazan kısım diode-node.info komutundan sonra sunucudaki çıktıda var. Aşağıya ekledim. NODEADI nasıl adlandırmak isterseniz o şekilde. İstediğiniz kadar node ekleyebilirisiniz aynı şekilde herhangi bir sınır yok.
```
register node NODEID NODEADI
```
![image](https://github.com/user-attachments/assets/22dd0c02-cfec-4188-b5ab-7133938685c7)


![image](https://github.com/user-attachments/assets/0075b3a1-f4ea-4f93-ad02-740094562a80)

### 🔹 14. Aşağıdaki iki bağlantı da sorunsuzdur. İlki gibi de görünebilir. Bundan sonrasını https://diodenetwork.io/app/ sitesinden de takip edebilirsiniz.

![image](https://github.com/user-attachments/assets/744efc57-1ed9-44c9-aedf-a7213da7557d)

![image](https://github.com/user-attachments/assets/1d1b8092-7e8f-41ff-bcc8-c77895c234e7)


### 🔹 15. Bazı yararlı sunucu kodları.

```snap install diode-node``` - yüklemek için

```diode-node.info``` - kurulu nodun bilgileri için

```snap restart diode-node``` - yeniden başlatmak için

```sudo snap logs diode-node -f``` - logları görmek için

### 🔹 16. Bazı yararlı Diode Collab registar kanalı komutları.

```stats``` - genel bilgilerinizi görmek için

```list nodes``` - kayıtlı tüm nodelarınızı görmek için.








