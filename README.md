# UÇUŞ KONTROL BİLGİSAYARLARI (AVİYONİK SİSTEM)

Ana aviyonik sistem, roket apogeeye ulaştığında MPL3115A2 basınç sensörü ile ölçtüğümüz, roketin son yüksekliği ile bir önceki yüksekliği verilerini birbirinden çıkardığımızda negatif sonuç eldersek ve MPU9255 IMU modülü ile roketin havadaki pozisyonunu inceleyerek istediğimiz şartları sağladığımızda Arduino Nano, röleyi 5V ile tetikleyerek karabarut yuvasına bağlı filiti ateşleyecektir ve roketin burnunun ayrılmasını sağlayacaktır.Bu sayede faydalı yük bırakılacaktır ve sürüklenme paraşütü açılacaktır.Eğer ana aviyonik sistem bu işlemi gerçekleştiremezse yedek aviyonik sistemimizdeki MQ-2 gaz sensörleri ortamda gaz olup olmadığnı tespit edecektir.Eğer ortamda gaz yok ise yedek aviyonik sistem, ana aviyonik sistemin başarısız olduğunu anlayarak BMP280 basınç sensörü ve MPU6050 IMU modülü ile belirlediğimiz şartları kontrol ederek röleyi tetiklecektir.Böylelikle ayrılma gerçekleşecek ve sürüklenme paraşütü açılacaktır.Ardından roket düşüşe geçtiğinde son 600 metrede tekrardan röleyi tetikleyerek karabarut patlaması sonucu ikinci ayrılmayı gerçekleştirecektir ve ana paraşüt açılarak roket yere sağlam bir şekilde inecektir.Roket yere indiğinde GY-NEO6MV2 GPS Modülü ile roketin konumu tespit edilecektir.Aviyonik sistemlerimizde ve faydalı yükümüzde bulunan sensörlerden ve modüllerden aldığımız bütün veriler LoRa E32-868T30D iletişim modülü ile yazılımını kendimizin yapcağı yer istasyonumuza iletilecektir.



ANA UÇUŞ BİLGİSAYARI

![yedek2 3d](https://user-images.githubusercontent.com/93153349/151841297-21f8e78a-0f0c-413a-a3b1-14bb911d6555.PNG)

![yedek2 şematik](https://user-images.githubusercontent.com/93153349/151841441-12c541c3-4808-417a-9339-c9f88feca643.PNG)





YEDEK UÇUŞ BİLGİSAYARI

![ana2 3d](https://user-images.githubusercontent.com/93153349/151841349-b6f991c6-c207-4caa-99ae-ab15c5dddc3f.PNG)

![ana2 şematik](https://user-images.githubusercontent.com/93153349/151841476-e888ec01-d9ad-4ffa-b177-a8aa1653d913.PNG)





FAYDALI YÜK

![yük 3d](https://user-images.githubusercontent.com/93153349/151841523-54fe51d4-c28b-4af6-a263-7a1d1929a26c.PNG)

![yük şematik](https://user-images.githubusercontent.com/93153349/151841538-4dd141e2-54c5-4f11-8d77-b9af48f6c779.PNG)
