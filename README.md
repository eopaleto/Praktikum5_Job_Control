![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/073abb7f-c1d6-41f3-96e0-6d0a5d5bf99c)


**1. Eksekusi seluruh profile yang ada :**     
      a. Edit file  profile  /etc/profile  dan  tampilkan pesan  sebagai berikut  :    `echo  “Profile dari /etc/profile”`
   
![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/f5abb259-fd38-45a7-a6f5-b2c6e2f55115)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/876a246c-63b3-45ae-bdc4-6455a44b789f)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/4391d241-a213-47e9-90d8-068911fe353d)

b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :   
- `/home/stD02001/.bash_profile`    
 ![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/ed0c6b27-0a5b-4d82-9f22-68d1c8483f1f)   
- `/home/eo/.bash_login`   
![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/81dc1229-f4b6-456c-8328-97b83a3d81e0)   
- `/home/eo/.profile`   
![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/3a25c2f8-9c08-4d60-95ed-6a2dc3a0d761)   
- `/home/eo/.bashrc`   
![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/e212874f-2078-435e-a045-fb0f1811cae4)   

  Ganti nama  /home/mahasiswa dengan nama anda sendiri. Pada  setiap  file tersebut, cantumkan  instruksi  echo,  misalnya  pada  /home/  mahasiswa/.bash_profile  :    echo “Profile dari .bash_profile”

c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:      

- Merubah file-file menjadi file executeable  
  ![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/7a8d2f71-e756-4239-964d-258cbc7579af)

- Menampilkan file-file yang dibuat  
  ![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/b0089edd-a62b-4b9f-842a-d4b94ff40201)

- `$ su eo`  
  `$ exit`
  
![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/8228c745-2a66-4492-99e4-cf2b037d011b)

- `$ su - eo`  
  `$ exit`  

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/3e941d06-ec81-4458-8be9-44a51cb09371)

**2. Prompt String (PS)**
a. Edit file  .bash_profile, ganti prompt PS1 dengan ‘>’.  Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell   

		`PS1=’> ‘`
		`export PS1`

b. Eksperimen hasil PS1 :   
		- `$ PS1=“\! > “`    
		  `69 > PS1=”\d > “`   
		  `Mon Sep 23 > PS1=”\t > “`    
		  `10:10:20 > PS1=”Saya=\u > “`   
		  `Saya=mahasiswa > PS1=”\w >”`   
		  `~ > PS1=\h >”`

 ![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/fe3572ed-3c79-4a40-84cf-87715ccbd54c)

**3. Logout**   

Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout   
  `Echo “Terima kasih atas sesi yang diberikan”`  
	`Sleep 5`   
  `clear`

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/169a5df2-b63f-450a-bb43-d13ff2457086)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/ff52e62f-d545-4ee0-bd33-7848280e57a8)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/31fa4e53-af83-40d5-ab5d-06f2e43267a1)

**4. Bash Script**
a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :  
  `p1.sh`  
  `#! /bin/bash`    
	`echo “Program p1”`    
  `ls –l`  

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/fc1b46f2-a960-4407-a720-8934a7a83bb9)

  `p2.sh`  
  `#! /bin/bash`    
	`echo “Program p2”`    
  `ls –l`  

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/05223ec3-b031-4d3d-ab90-cbd5f596d5cf)

  `p3.sh`  
  `#! /bin/bash`    
	`echo “Program p3”`    
  `ls –l`  
 
![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/de2da7b2-5e11-46a0-88b8-2cc8e258f4e3)

b. Jalankan script tersebut sebagai berikut :   
	- execute file agar bisa dijalankan

 ![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/f4932296-93c5-4ccf-af70-ad6e4fa407df)


![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/29345987-9789-44f6-b2dd-34fb9556fb2c)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/b0119352-6a9d-4364-b9fe-d928abc9674d)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/882d6739-9a0f-45ba-b56d-238380797b90)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/1b7b96b7-bb7e-40f7-beb6-e7a19ad4f384)

**5. Job**

a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh,  setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.


![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/b0cb7217-b3a6-4539-9dee-c92b7668699c)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/eeceb0c3-ee73-4451-aefe-5e9f75ee9528)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/aa4d9b14-e916-4121-a569-d70afceb2197)

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/22f14388-a2c5-4831-b048-a3c43aa26093)

**6. History**
a. Ganti nilai HISTSIZE dari 1000 menjadi 20   

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/79287b3a-4a4a-4881-b791-a755e19a136e)

b. Gunakan  fasilitas  history  dengan  mengedit  instruksi  baris  ke  5  dari  instruksi  yang terakhir dilakukan

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/a44e866d-a215-43e3-b3cb-a4ae1f399990)

c. Ulangi instruksi yang terakhir.  Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer  

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/5a9cca6a-ea35-4069-aa13-525a59cfb8a7)

d. Ulangi instruksi pada history bufer nomor 150

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/34b71f0a-1afc-4635-af75-bcfa774f2da2)

e. Ulangi instruksi dengan prefix “ls”   

![image](https://github.com/eopaleto/Praktikum5_Job_Control/assets/126212773/072bd121-f375-4be5-afd2-6eddfdb583cd)
