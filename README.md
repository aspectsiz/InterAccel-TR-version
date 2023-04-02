### [ Download Latest Version.](https://github.com/KovaaK/InterAccel/releases/latest)
[![Screenshot 1](https://i.imgur.com/4vy7XYf.png)](https://github.com/KovaaK/InterAccel/releases/latest)
# Interception Acceleration

Bu program, QuakeLive tarzı fare hızlandırmasını, oyunun RawInput, DirectInput veya başka bir şey kullanıp kullanmadığına bakılmaksızın, işletim sistemi ve herhangi bir oyunda kullanmanıza olanak tanır. Fare hareketlerini işletim sistemine göndermeden önce yakalamak ve QL'nin yaptığı matematiğe göre değiştirmek için Interception Sürücüsünden yararlanır.

Yüklemek için gerekenler:

1. "interception" klasöründen "install_driver.bat" dosyasını çalıştırarak "interception" sürücüsünü yükleyin (Yönetici ayrıcalıkları isteyecektir).
2. Eğer yoksa, https://www.microsoft.com/tr-tr/download/details.aspx?id=48145 adresinden Visual Studio 2015 için Visual C++ Redistributable'ı yükleyin.
3. Bilgisayarınızı Yeniden başlatın. Evet, gerçekten ilk adımdan dolayı yeniden başlatmanız gerekiyor, aksi takdirde çalışmaz.

Yeniden başlatıldıktan sonra, bir "uygulama" klasörlerinden birine giderek interGUI.exe'yi çalıştırabilirsiniz. Program, fare hızlandırması için bir başlangıç noktası vermek için yapılandırma sihirbazını çalıştıracaktır, ancak tercih ettiğiniz herhangi bir ayarı kullanabilirsiniz.

Bu sürücüyle ilgili en kapsamlı ve güncel kılavuz için N.R.K'nın GDoc'una bakın.

Önemli notlar:

╚ Interaccel.exe, gerçek zamanlı fare hızlandırmasını gerçekleştiren programdır ve ilk kez çalıştırıldığında yapılandırma değerlerini yalnızca okur.

╚ InterGUI.exe, Interaccel.exe'yi arka planda çalıştırır ve yapılandırma değerleri değiştirildiğinde otomatik olarak kapatır/yeniden başlatır.

╚ InterGUI.exe veya Interaccel.exe'yi kapatırsanız, Interception sürücüsü tarafından HERHANGİ bir fare hızlandırması uygulanmaz ve girdileriniz sürücüyü yüklemediyseniz aynı olacaktır.

╚ InterGUI.exe'yi görev çubuğuna küçültebilirsiniz ve çalışmaya devam eder. Ayrıca programı Windows'ta otomatik olarak başlayacak şekilde programlayabilir ve simge durumuna küçültülmüş şekilde başlamaya zorlamak için komut satırı parametrelerine "-m" ekleyebilirsiniz.

╚ settings.txt dosyasında "FancyOutput" adlı gizli bir ayar vardır. "1" olarak ayarlandığında, interaccel.exe'yi doğrudan çalıştırırsanız gerçek zamanlı hassasiyet/hızlandırma çıktısını gösterebilir. Ancak az miktarda giriş gecikmesi oluşur, bu nedenle GUI her devraldığında FancyOutput'u 0'a zorlar.
