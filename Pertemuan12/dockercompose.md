## Deploy Multiple Container menggunakan Docker Compose

1. Start Instance EC2 di AWS

2. Patching OS

3. Uninstall semua Services manual sebelumnya

4. Repositori baru untuk web dinamis di docker hub alt text
   ![alt text](<Screenshot 2026-05-19 042057.png>)
5. Buka Projek Company himafor_nim

6. Bagi 2 Folder untuk projek Web App Statis dan Dinamis

7. Move file index dan Dcoker milik web statis ke Folder web-statis

8. Copy Folder Projek Next.JS (pertemuan9)ke folder web-dinamis

9. Lakukan Testing di Local Project Next.JS

Install Dependencies: npm install
Create user di DBMS : sudo mysql -u root -p
CREATE USER 'userwebdinamis*2388010027'@'localhost' IDENTIFIED BY '3nS]9gnbU[nBP[Gw';
GRANT ALL PRIVILEGES ON *.\_ TO 'userwebdinamis_2388010027'@'localhost';
FLUSH PRIVILEGES;
exit;
![alt text](<Screenshot 2026-05-19 060648.png>)
Edit File .env di folder web-dinamis
npm run build
npm start
Pastikan web dapat diakses di http://localhost:3000 admin tanpa error
![alt text](<Screenshot 2026-05-19 061434.png>) 10. Buat file Dockerfile

11. Buat file docker-compose.yml

12. Buat Workflows File -> deploy-dinamis.yml di folder .github/workflows/ dari Projek web-dinamis

13. Edit File -> deploy.yml di folder .github/workflows/ untuk

14. Update Host AWS di Github

15. Comit Changes ke GitHub dari lokal

16. Push Changes ke GitHub

17. Cek di Github, apakah actions jalan dan berhasil
    ![alt text](<Screenshot 2026-05-19 090201.png>)

18. Cek di AWS, apakah container berjalan dengan baik alt text

19. Akses web melalui Browser login admin edit Layanan alt text
    ![alt text](<Screenshot 2026-05-19 093538.png>)
    Referensi :

https://github.com/moh-firdaus/himafor_nim
