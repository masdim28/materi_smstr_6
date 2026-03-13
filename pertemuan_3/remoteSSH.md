1. unduh dan Install Putty di https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html
   ![alt text](image.png)
2. Konversi ekstensi Private Key dari .pem menjadi .ppk

Buka Putty Gen
Load Private Key .pem
Klik Save Private Key menjadi ekstensi File .ppk

![alt text](<Screenshot 2026-03-13 101818.png>) 3. Setting-Up Remote SSH dengan Putty

isi Ipv4 addres Public data berasal dari instance masing2
port SSH (22)
load private key .ppk di menu Connection->SSH->Auth->Credential
user dari instance masing-masing (ubuntu)
![alt text](<Screenshot 2026-03-13 110513.png>) 4. Setiap awal Remote kita lakukan Patching OS
sudo apt-get update && sudo apt-get upgrade

5. coba lakukan instalasi Web Server dalam keadaan Kosong
   ![alt text](<Screenshot 2026-03-13 111907.png>)
   instal salah satu web server sudo apt install nginx

![alt text](<Screenshot 2026-03-13 131646.png>)
karena ada kendala yg mengharuskan mematikan servernya jadi ip di ss an ini berbeda dengan ip di ss sebelumnya
