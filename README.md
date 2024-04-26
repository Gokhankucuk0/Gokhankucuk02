## Docker Compose Nedir?
Docker, yazılım geliştiricilerin, sistem yöneticilerinin ve yazılım dağıtım ekiplerinin iş akışlarını iyileştiren popüler bir araçtır.
Docker, ilk olarak 2013 yılında Solomon Hykes tarafından geliştirildi ve 2013 yılının Mart ayında ilk kez duyuruldu. Docker, o zamandan beri sürekli olarak geliştirilmiş ve yaygın olarak kullanılan bir yazılım haline gelmiştir.

Multi-container: Bu terim tek bir uygulamanın birden fazla docker container’ı kullanarak çalışması anlamına gelir.

Docker Compose Tanımlamak ve Kullanmak
Docker Compose’u kullanmak 3 adımlı bir işlemdir.

1.ADIM:
Uygulamanın environmentini bir dockerfile ile tanımlayın. Bu sayede istediğiniz her yerde üretilebilir.
Dockerfile: Bir dockerfile, bir uygulamanın nasıl oluşturulacağı ve çalıştırılacağı hakkında talimatlar içeren bir dosyadır. Bu dosya, uygulamanızın çalışma ortamını tanımlar. (İşletim sistemi, programlama dili sürümleri, kütüphaneler, ortam değişkenleri v.s.) Dockerfile kullanarak, uygulama herhangi bir sistemde ya da cloud ortamında aynı şekilde sorunsuz bir şekilde çalıştırılabilir. Bu yaklaşım farklı ortamlarda (dev, test, prod) tutarlı bir şekilde çalışmasını sağlar. Bu durum da aslında “lokalimde çalışıyordu” cevabını olabildiğince minimuma indirir. (:
Docker, bu dockerfile’daki talimatları ,zleyerek b,r Docker imajı oluşturur. Ve bu imaj daha sonra farklı makinelerde Docker containerları olarak çalıştırılabilir. Bu sayede; uygulamanın, herhangi bir yerde aynı konfiglerle yeniden üretilebilmesi sağlanmış olur.

2.ADIM:
İzole edilmiş bir ortamda birlikte çalıştırılabilmeleri içi uygulamayı oluşturan servisleri bir compose.yaml dosyasında tanımlayın.

3.ADIM
docker-compose dosyasının bulunduğu dizinde docker compose up komutu ile compose dosyanızı çalıştırın


