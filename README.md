# Tugas6_Pratikum5_Sistem-Operasi

1. Eksekusi seluruh profile yang ada :
   a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut : echo “Profile dari /etc/profile”

   <img width="1280" height="800" alt="1 a ubuntu" src="https://github.com/user-attachments/assets/181330b9-e831-466e-ae19-70ffa8ed6585" />
   <img width="1280" height="800" alt="1a ubuntu" src="https://github.com/user-attachments/assets/78cb1529-768b-4c90-93a7-877ce4d433f4" />

   b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :
   /home/stD02001/.bash_profile
   /home/. stD02001/.bash_login
   /home/mahasiswa/.profile
   /home/mahasiswa/.bashrc
   Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap   file tersebut, cantumkan misalnya pada /home/mahasiswa/.bash_profile :
   echo “Profile dari .bash_profile”
   Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan. 

   <img width="1280" height="800" alt="1b nano ubuntu1" src="https://github.com/user-attachments/assets/8dd9fe77-1237-4033-aaa9-d5779d797208" />

   <img width="1280" height="800" alt="1b nano ubuntu2" src="https://github.com/user-attachments/assets/28116c45-a50a-45fd-86bc-e53b4805c070" />

   <img width="1280" height="800" alt="1b ubuntu3" src="https://github.com/user-attachments/assets/35aae2ef-86ca-4eca-9ed3-00d7d55ac8e3" />

   <img width="1280" height="800" alt="1b nano ubuntu4" src="https://github.com/user-attachments/assets/f69f025c-1508-4810-a7f6-b61d79502b9c" />

   <img width="1280" height="800" alt="1b ubuntu" src="https://github.com/user-attachments/assets/53caa048-411b-48a7-b3fa-1e74375a7e37" />

   c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:
   $ su mahasiswa
   $ exit
   kemudian gunakan opsi – sebagai berikut :
   $ su – mahasiswa
   $ exit
   Jelaskan perbedaan kedua utilitas tersebut.

   <img width="1280" height="800" alt="ubuntu 1C" src="https://github.com/user-attachments/assets/c91c1eb4-8cc4-47f3-afe2-14450ef0c10e" />


2. Prompt String (PS)
   a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan
   variable PS1 dikenal oleh semua shell
   PS1=’> ‘
   export PS1

   <img width="336" height="332" alt="2A BENER" src="https://github.com/user-attachments/assets/b843e09c-0c7b-48ff-9956-90087ac6f0ab" />

   <img width="1280" height="800" alt="2A" src="https://github.com/user-attachments/assets/c6fa6d7a-cfa0-4d38-8982-c5449dd64429" />

   b. Eksperimen hasil PS1 : $ PS1=“\! > “   69 > PS1=”\d > “   Mon Sep 23 > PS1=”\t > “   10:10:20 > PS1=”Saya=\u > “  Saya=mahasiswa > PS1=”\w 
   >”  ~ > PS1=\h >”

   <img width="564" height="294" alt="2b ubuntu" src="https://github.com/user-attachments/assets/fd1c45db-aff0-47d1-ac82-2bcce187ac0b" />


3. Logout Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout
   Echo “Terima kasih atas sesi yang
   diberikan”
   Sleep 5
   clear

   <img width="1280" height="800" alt="VirtualBox_ubuntu26_13_10_2026_10_45_54" src="https://github.com/user-attachments/assets/953b9328-3367-43d9-96e3-63b0505f1df1" />

   <img width="471" height="159" alt="VirtualBox_ubuntu26_13_10_2026_10_33_29" src="https://github.com/user-attachments/assets/dff1d4f1-d8d0-49cc-becf-372d08d13a0e" />


   




   









   
