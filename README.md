Nama : Raden Kodrat

Kelas : TI.20.D.1

NIM : 312010271

matkul : Sistem Basis Data

.Masuk ke databse nama_nim

![Database](https://user-images.githubusercontent.com/101814131/174483374-2bacb7ca-9968-47d4-b48a-6fc486ed26f6.PNG)


. Lakukan proses backup dan recovery dengan sql dari database tugas seblumnya !

backup

![Database](https://user-images.githubusercontent.com/101814131/174483472-72eda445-9bdf-4d0e-8220-04603e0945c1.PNG)




Jika proses backup berhasil maka akan muncul file backuppada direktori C:\xampp\mysql\data\nama database
![Capture](https://user-images.githubusercontent.com/101814131/174483503-36d2f122-0ac8-48b7-a538-5d6439f70a27.PNG)


Recovery

Data yang telah di-backup dapat dikembalikan kapan saja bila diperlukan. Sintaks SQL yang digunakan adalah LOAD DATA INFILE. Perintah yang dijalankan adalah

LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ;
![2](https://user-images.githubusercontent.com/101814131/174483538-04af65e1-ae84-4fe9-a7ab-59b4c56a028f.PNG)
![3](https://user-images.githubusercontent.com/101814131/174483564-6a56b096-7e95-4489-8c78-8cb7eaf64cdd.PNG)


. Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnya !

![4](https://user-images.githubusercontent.com/101814131/174483632-e67a78e2-efa7-4dbb-a718-7822a69e9438.PNG)


Tulisakan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !

crontab –e

00**7myqldump -u root -p aldi_312010008>aldi_312010001_backup.sql
![5](https://user-images.githubusercontent.com/101814131/174483641-3f946810-3ecd-4c53-9908-cf50b4ed2e2c.PNG)
