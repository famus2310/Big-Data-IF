# Tugas 5

## Fadhil Musaad
## 05111740000116

# Apache Spark Cluster menggunakan Docker

## Tahapan

### Instalasi Docker Compose
1. Instalasi docker-compose menggunakan `sudo curl -L "https://github.com/docker/compose/releases/download/1.25.5/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose`
2. Buat permission pada docker-compose dengan command `sudo chmod +x /usr/local/bin/docker-compose`
3. Periksa versi docker-compose menggunakan command `docker-compose --version` akan terlihat seperti berikut ![docker-version](img/docker-version.png)

### Membuat Apache Spark Cluster
1. Download file docker compose dengan command `wget https://raw.githubusercontent.com/bitnami/bitnami-docker-spark/master/docker-compose.yml`
2. lalu jalankan perintah `docker-compose up` untuk membuat container
3. Tunggu hingga proses selesai ![docker-compose](img/docker-compose.png)
4. Periksa daftar container menggunakan command `docker ps` ![docker-container](img/docker-container.png)
5. Test Spark Cluster dengan mengakses http://localhost:8080 pada browser ![spark-cluster](img/spark-cluster.png)

### Menjalankan Script Python pada Apache Spark Cluster
1. Lakukan perintah `docker exec -it <id-container-master> /bin/bash`
2. Periksa alamat ip menggunakan `hostname -i`
3. Submit job dengan menggunakan command `spark-submit --master spark://<alamat-ip>:<port> <source-file> <jumlah-partisi>`

### Mencoba dengan Parameter yang Lebih Besar
1. Lakukan submit job dengan jumlah partisi 1000
2. Bandingkan Completed Applications pada web browser ![parameter](img/compare.png)
Untuk 10 Partisi:
![10](img/10.png)

Untuk 1000 Partisi:
![1000](img/1000.png)

### Percoban dengan Paramter yang Berbeda
 
