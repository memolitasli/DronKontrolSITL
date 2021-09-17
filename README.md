# DronKontrolSITL

# Gerekenler
* Dronekit  (https://dronekit-python.readthedocs.io/en/latest/develop/installation.html) 
* Ardupilot (https://ardupilot.org/dev/docs/building-setup-linux.html)
* Tkinter ($ pip install tk)
* Mission Planner veya herhangi bir başka GCS yazılımı
* Pyrebase (Firebase bağlantısı için)

# Nasıl Kullanılır
  
  # Kalkış
  Terminal ekranında kodu çalıştırdıktan sonra sizden bağlantı adresini isteyecek STIL için 'udp:127.0.0.1:14551'
  Kalkış yapmak için Y tuşuna basın ve terminal ekranına istediğiniz irtifa degerini girin
  
  # Sürüş
  * Klavyede bulunan ok tuşlarını kullanarak dronu hareket ettirebilirsiniz.
  * W tuşu ile dronu yükseltebilir, S tuşu ile alçaltabilirsiniz
  * B Tuşuna basarak o anda bulunduğunuz konuma ait enlem , boylam ve irtifadeğerlerini ekrana yazdırabilirsiniz.
  * R Tuşuna basarak dron RTL moduna girer kalkışa eçtiği konuma geri döner ve iniş yapar, tekrardan Y tuşuna basarak kalkışa geçebilirsiniz.
  * L Tuşu dronu bulunduğu konuma indirir ve size tekar kalkmak veya görev belirlemek olarak 2 seçenek sunar
  * E Tuşuna basarak firebase'e kaydettiğiniz enlem , boylam ve irtifa değerlerini indirebilir ve dronu sırasıyla bu konumlara gönderebilirsiniz
  
  # Görev Belirleme
  GCS (Bu durumda mission Planner) üzerinde plan kısmına girin ve istediğiniz konumlara tıklayın
  bu konumlar dronunuzun gideceği konumları belirtir. Daha sonra write butonuna basarak bu konumları drona yazınız.
  Uçuş yazılımımız tarafılan açılan beyaz pencerede L tuşuna başın ve dronu yere indirin, daha sonra Gorev belirle seçeneğini seçin
  Dron tüm noktaları dolaştıktan sonra kalkış yaptığı yere geri dönecek
  **Görev tamamlandıktan sonra uçuşa ait bilgiler ucusVerileri.txt adında bir dosyaya yazılacak**
  # Firebase
  * Firebase üzerinden bir realtime database oluşturun 
  * Database oluştururken size verilen config verilerini kod içerisindeki ilgili yere yapıştırın 
  * ekleyeceğiniz verilerin isimleri enlem,boylam ve irtifa olmalı
  * Dron havalandıktan sonra E tuşuna basarak bu verileri indirebilir ve dronu sırasıyla bu konumlara gönderebilirsiniz. 
  * Görev belirlemede olduğu gibi dron en son olarak görevin indirildiği konuma geri dönecektir.
  
