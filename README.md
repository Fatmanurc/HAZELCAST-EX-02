# HAZELCAST-EX-02

Bu ödevde Docker Compose kullanılarak **Hazelcast cluster** ve **Hazelcast Management Center** kurulumu yapılmıştır. Ödevin amacı, containerların lokal ortamda çalıştırılması ve Management Center üzerinden cluster durumunun görüntülenmesidir.

##  Kurulum ve Çalıştırma Adımları

1. **Proje klasörü oluşturun ve docker-compose.yml dosyasını ekleyin**

mkdir Hazelcast-Exercise
cd Hazelcast-Exercise

2. **Docker Compose ile containerları başlatın**

docker-compose up -d

3. **Çalışan containerları kontrol edin**

docker ps

4. **Hazelcast loglarını kontrol edin**

docker logs hazelcast_member

5. **Management Center üzerinden cluster’ı görüntüleyin**

-Tarayıcıdan şu adresi açın: http://localhost:8080

-İlk açılışta “Connect to Cluster” veya benzeri bir seçenek görebilirsiniz.

-Cluster adı: dev-cluster (docker-compose.yml’de belirlenen isim).

-Dashboard’da Hazelcast node’u görüntülendiğinde her şey çalışıyor demektir.
