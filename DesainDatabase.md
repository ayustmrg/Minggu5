# Design Database With MySQL  

**Menentukan Entity**  
* Berdasarkan requirement yang ada kita bisa mulai untuk mengidentifikasi entity dalam database.  
* Beberapa kandidat yang paling sering menjadi sebuah entity : peoples, things, events, locations  
* Mari kita lihat kembali requirement yang ada, dan kita mulai list entity yang ada.  
* Berikut adalah kandidat yang bisa dijadikan enitity dalam database : user, singer, track, album, playlist  

</br>

**Menentukan Atribbutes dari Entity**  
* Tahapan ini kita akan menentukan attributes apa saja yang akan datanya kita simpan di dalam sebuah entity.  
* Attributes yang di perlukan didalam entity kemungkinan sudah ada di dalam requirements document, atau mungkin juga diperlukan penafsiran kita sendiri sebagai database developer.  

**User Entity**  

<img src="de1.jpg" width="200" height="100">  


**Singer Entity**  

<img src="de2.jpg" width="200" height="100">  


**Track Entity**  

<img src="de3.jpg" width="200" height="100"> 


**Album Entity**

<img src="de4.jpg" width="200" height="100">  


**Playlist Entity**

<img src="de5.jpg" width="200" height="100">  

</br>

**Menentukan Relasi Antar Entity**  
* Didalam requrement mungkin sudah dijelaskan relasi dari beberapa entity.  
* Namun terkadang didalam requirement juga tidak dijelaskan mengenai relasi, dan kita sebagai database developer menafsirkan relasi antar entity


**Relasi Entity Singer dan Entity Track**   
*  1 singer punya 1 atau lebih track  
* Relationshipnya adalah one to many

<img src="de6.jpg" width="200" height="100">  


**Relasi Entity Album dan Entity Track**  
* 1 Album punya 1 atau lebih track  
* Relationshipnya adalah one to many

<img src="de7.jpg" width="200" height="100">  


**Relasi Entity User dan Entity Playlist**  
* 1 User punya 0 atau lebih Playlist  
* Relationshipnya adalah zero or more to many

<img src="de8.jpg" width="200" height="100">  


**Relasi Entity Playlist dan Entity Track**  
* 1 Playlist punya 1 atau lebih Track  
* 1 Track bisa ada di banyak playlist  
* Relationshipnya adalah many to many  
* Untuk relasi many to many, kita butuh entity tambahan sebagai penghubung, (conjunction)

<img src="de9.jpg" width="200" height="100">

**Relasi Entity Playlist dan Entity Track**  
Relasi asli :  

<img src="de10.jpg" width="200" height="100"> 

Conjusction

<img src="de11.jpg" width="200" height="100">  

</br>

**Relationship Entity Keseluruhan**  

<img src="de12.jpg" width="200" height="100">    

</br>

**Membuat SQL Table dari Entity**  
* Setelah kita punya ERD, maka kita akan lanjut dengan create table berdasarkan dengan data yang kita punya.  
* Pada kali ini kita akan menggunakan terminal untuk menjalankan query SQL  


**Membuat Table User**  

<img src="de13.jpg" width="200" height="100">  

<img src="de14.jpg" width="200" height="100">  


**Membuat Table Singer**  

<img src="de15.jpg" width="200" height="100">  

<img src="de16.jpg" width="200" height="100">  


**Membuat Table Album**

<img src="de17.jpg" width="200" height="100">  

<img src="de18.jpg" width="200" height="100"> 


**Membuat Table Track**

<img src="de19.jpg" width="200" height="100">  

<img src="de20.jpg" width="200" height="100">  

<img src="de21.jpg" width="200" height="100">  


**Membuat Table Playlist**

<img src="de22.jpg" width="200" height="100">  

<img src="de23.jpg" width="200" height="100">  


**Membuat Table Playlist_Track**

<img src="de24.jpg" width="200" height="100">  

<img src="de25.jpg" width="200" height="100">  