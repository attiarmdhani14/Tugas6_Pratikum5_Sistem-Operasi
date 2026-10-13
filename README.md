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

   su username : beralih ke pengguna lain tanpa melalui lingkungan login secarah penuh.

   su - username : Beralih ke pengguna lain dengan lingkungan login, termasuk pengaturan lingkungan dan pembacaan file profile login yang sesuai.


3. Prompt String (PS)
   a. Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan
   variable PS1 dikenal oleh semua shell
   PS1=’> ‘
   export PS1

   <img width="336" height="332" alt="2A BENER" src="https://github.com/user-attachments/assets/b843e09c-0c7b-48ff-9956-90087ac6f0ab" />

   <img width="1280" height="800" alt="2A" src="https://github.com/user-attachments/assets/c6fa6d7a-cfa0-4d38-8982-c5449dd64429" />

   b. Eksperimen hasil PS1 : $ PS1=“\! > “   69 > PS1=”\d > “   Mon Sep 23 > PS1=”\t > “   10:10:20 > PS1=”Saya=\u > “  Saya=mahasiswa > PS1=”\w 
   >”  ~ > PS1=\h >”

   <img width="564" height="294" alt="2b ubuntu" src="https://github.com/user-attachments/assets/fd1c45db-aff0-47d1-ac82-2bcce187ac0b" />


4. Logout Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout
   Echo “Terima kasih atas sesi yang
   diberikan”
   Sleep 5
   clear

   <img width="1280" height="800" alt="VirtualBox_ubuntu26_13_10_2026_10_45_54" src="https://github.com/user-attachments/assets/953b9328-3367-43d9-96e3-63b0505f1df1" />

   <img width="471" height="159" alt="VirtualBox_ubuntu26_13_10_2026_10_33_29" src="https://github.com/user-attachments/assets/dff1d4f1-d8d0-49cc-becf-372d08d13a0e" />


5. Bash script
   a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :
   p1.sh
   #! /bin/bash
   echo “Program p1” ls –l
   p2.sh
   #!/bin/bash
   echo “Program p2” who
   p3.sh
   #! /bin/bash
   echo “Program p3” ps x

   <img width="1280" height="800" alt="4A" src="https://github.com/user-attachments/assets/c7132e61-8364-47ec-8444-da43b6558955" />

   b. Jalankan script tersebut sebagai berikut :
   $ ./p1.sh ; ./p3.sh ; ./p2.sh
   $ ./p1.sh &
   $ ./p1.sh $ ./p2.sh & ./p3.sh &
   $ ./p1.sh ; ./p3.sh ) &

   <img width="1280" height="800" alt="4A2" src="https://github.com/user-attachments/assets/a5c4b3ce-2b31-4093-acdb-0c13cf69fb34" />

   <img width="1280" height="800" alt="4A3" src="https://github.com/user-attachments/assets/e19da0cc-d4ab-47af-8209-eff5bec38c46" />

   <img width="1280" height="800" alt="4A4" src="https://github.com/user-attachments/assets/ef24c75b-4746-4c19-8c6b-f008d455f30b" />

   <img width="1280" height="800" alt="4A5" src="https://github.com/user-attachments/assets/7353c6f6-73c2-41df-9be5-36cd78846519" />


6. Jobs
   a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.
   #!/bin/bash
   while [ true ]
   do
    date >> hasil
    sleep 10
   done

   <img width="1280" height="800" alt="5A" src="https://github.com/user-attachments/assets/3c74df4f-e4b6-49ff-8475-dca98d7c77e2" />

   <img width="449" height="66" alt="5A2" src="https://github.com/user-attachments/assets/ac0b911f-a9c1-4165-98a2-ae1de32ccf00" />
   

   b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :
   $ jobs
   $ find / -print > files 2>/dev/null &
   $ jobs

   <img width="645" height="302" alt="5B" src="https://github.com/user-attachments/assets/bd2e6863-34e4-4749-8569-df3db5f28fba" />


   c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background
   $ fg %1
   $ bg

   <img width="699" height="248" alt="5C" src="https://github.com/user-attachments/assets/fe0fb14f-baf9-4ccc-94ec-3b33b8c81a48" />


   d. Stop program background dengan utilitas kill
   $ ps x
   $ kill [Nomor PID]

   <img width="1219" height="595" alt="5D1" src="https://github.com/user-attachments/assets/f3b1b251-98e3-414d-b8e5-0afec409ebe8" />

   <img width="459" height="79" alt="5D2" src="https://github.com/user-attachments/assets/c4ece1f4-3a47-4583-bade-84f65f44c48c" />


7. History
   a. Ganti nilai HISTSIZE dari 1000 menjadi 20
   $ HISTSIZE=20
   $ h

   <img width="1280" height="800" alt="6A" src="https://github.com/user-attachments/assets/d3001e2c-7d3b-4d5d-9308-7179c41b5c24" />
   

   b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan
   $ !-5

   <img width="1280" height="800" alt="6B" src="https://github.com/user-attachments/assets/6774677b-932b-468a-a07b-63d4147be2e0" />


   c. Ulangi instruksi yang terakhir.  Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer
   $ !!

   <img width="1280" height="800" alt="6C" src="https://github.com/user-attachments/assets/66b95bc3-26a3-4ea8-adb6-c3fa38b5b19e" />


   d. Ulangi instruksi pada history bufer nomor 150
   $ !150

   <img width="1280" height="800" alt="6D" src="https://github.com/user-attachments/assets/ab9eb350-e400-47ff-b6e8-333aef5ce15b" />


   e. Ulangi instruksi dengan prefix “ls”
   $ !ls

   <img width="1280" height="800" alt="6E" src="https://github.com/user-attachments/assets/993e26d3-54ed-4ac0-88a6-aef7d54c6ef0" />









   


   




   









   
