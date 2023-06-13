# Task Version Control System

#### 1. Penjelasan Distributed Version Control
 DVS adalah Sistem yang dibentuk untuk membantu para developer mengelola repositori secara penuh dan meminimalisir misskomunikasi antar developer dalam mengubah source code dari waktu ke waktu.
#### 2. Buat repository sample (diluar tugas) yang berisi 3 file dengan isi yang berbeda
- Pertama-tama buat Repository di Git.Hub<br/><br/>![1 Create Repository](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/a5bb09e3-c1bb-409d-85d7-e4dec504ce9a)<br/><br/>
- Setelah membuat Repository, ketik command ``$ ssh-keygen`` untuk membuat keygen :<br/><br/>![2 ssh-keygen](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/73d31001-8595-4fbb-b4b6-e49144f479d8)<br/><br/>
- Ketik ``$ cd .ssh/ $ cat id_rsa.pub`` dan copy semua key id_rsa publik :<br/><br/>![4  Copy id_rsa](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/02a68f78-84e2-4a22-800a-06b329f43de6)<br/><br/>
- Buka setting dan pilih ``SSH and GPG keys`` dan pilih ``New SSH key``<br/><br/>![4 Copy SSH  Key](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/75a60e1c-c223-4629-a9af-9595685e298f)<br/><br/>![5  Add SSH Key](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/29bee7dd-db9b-4e96-b162-5d1bf0a06e3a)<br/><br/>
- Berikutnya lakukan Git Config, untuk mengkonfigurasi koneksi lokal ke Git.Hub. ``git config --global user.name "your.github-user.name"``,``git config --global user.email "your.github-user.email"``. Untuk mengecek dengan Command ``git config --list``<br/><br/>![6 Git Config](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/c67a8f26-e07a-4311-81e1-883aaaf409b3)<br/><br/>
- Membuat sebuah directory, masuk didalam directory dan buat perintah ``$ git init``<br/><br/>![8  Touch File](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/75337a76-04fc-49d6-b702-4183478613da)<br/><br/>
- Lakukan perintah ``$ git add .``, untuk mentandai file yang sudah direvisi dan belum dideploy ke Git.<br/><br/>![10  Git Add](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/6bc567f7-577f-4420-9aae-3d4a63a5aea4)<br/><br/>
- Berikutnya bila file sudah direvisi dan ingin disimpan di Git maka lakukan perintah ``$ git commit -m "pesan commit yang ingin kalian buat"``<br/><br/>![11 Git Commit](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/16477959-c02e-4ece-8160-527e9b30de54)<br/><br/>
- Setelah itu, lakukan perintah ``git remote add origin "your-SSH"``<br/><br/>![8 SSH](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/cb6a681d-179f-42c4-850d-4308205a4829)<br/><br/>![Add Git Remote](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/3dde48a8-5c56-486a-a21f-f2c691f7b7b1)<br/><br/>
- Cara mengecek remote yang kita gunakan dengan perintah berikut ``$ git remote -v``<br/><br/>![Check Remote](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/b1024f70-bea6-4eeb-97cd-5964676220aa)<br/><br/>
- Last Step, dengan Git Push fungsinya untuk mengupload data file yang kita sudah anggap sampai tahap finalisasi untuk dipush ke repository database Git server. dengan perintah berikut ``$ git push origin master``<br/><br/>![12  Git Push](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/8b2fc44d-3708-4814-9cba-946a7b8ba7ec)<br/><br/>
- Dan terakhir lakukan refresh ke Web pada tampilan Git SSH<br/><br/>![13  Final Refresh Web](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/cfa8ce6c-8aab-4c9e-a862-3c96444b8db5)<br/><br/>

#### 3. Buat 2 branch - Staging - Production

- Pertama buat perintah ``$git branch staging``<br/><br/>![1](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/1409f3aa-3153-4d91-9972-e762f752881e)<br/><br/>
- Kedua lakukan  perintah juga ``$ git branch production``, dan untuk mengecek list berapa branch yang kita miliki dengan perintah ``$ git branch -a``<br/><br/>![2](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/d46c05e3-fe42-4bec-bf7c-92442d9ea112)<br/><br/>
- Untuk berpindah branch dengan cara ``$ git checkout (name branch)``<br/><br/>![3](https://github.com/darblietz/devops17-dumbways--M-Yusuf-Haidar-Week-2-Version-Control-System/assets/98991080/c9f452da-273e-44fb-ac6a-bfeb5b5e331e)<br/><br/>
- <br/><br/><br/><br/>









#### 4. Cari 3 command git yang belum dijelaskan
