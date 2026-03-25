# Database Project- [Gym Management System]

## Системийн тайлбар

Энэхүү төсөл нь [Gym Management System] системийн өгөгдлийн санг зохион байгуулсан болно.

Систем нь дараах үндсэн хүснэгтүүдээс бүрдэнэ:

- Table 1: **members**
- Table 2: **trainers**
- Table 3: **subscriptions**
- Table 4: **attendance**

Эдгээр хүснэгтүүд нь хоорондоо *Foreign Key* холбоотой бөгөөд бодит системийн өгөгдлийг хадгалах зориулалтай.

## Ашиглах заавар (Run Instructions)

Дараах дарааллаар ажиллуулна:

1. MySQL server ажиллаж байгаа эсэхийг шалгана.
2. mysqlScript.sql файлыг нээнэ.
3. Бүх кодыг нэг дор ажиллуулна.

Үүний үр дүнд:

- Database үүснэ.
- Хүснэгтүүд үүснэ.
- Өгөгдөл орно.
- Query-үүд ажиллана.

Файлын бүтэц
image

### 5-р хэсэг: Хэрэглэгч ба эрх(User & Privileges)
create user 'admin_user'@'localhost' identified by 'Root@2026';
grant all privileges on gym_db.* to 'admin_user'@'localhost';
grant select on gym_db.* to 'report_user'@localhost';
flush privileges;
create user 'admin_user'@'localhost' identified by 'Report@2026';
grant all privileges on gym_db.* to 

### 6-р хэсэг: Backup & Restore
