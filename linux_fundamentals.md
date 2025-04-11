 Basic Commands / Основні команди
echo "text"     # prints text to the terminal / виводить текст у термінал
whoami          # shows current user / показує ім’я користувача
pwd             # print working directory / поточна директорія
ls -la          # list all files incl. hidden / всі файли, включно з прихованими
cd ..           # go up one directory / перейти на рівень вище

File Operations / Робота з файлами
touch file.txt      # create empty file / створити порожній файл
mkdir test_dir      # create directory / створити каталог
rm file.txt         # remove file / видалити файл
mv old new          # rename/move / перейменувати або перемістити
cp source dest      # copy files / копіювати файли

Permissions / Права доступу
ls -l                   # show permission flags / показує права доступу
chmod +x file.sh        # add execute permission / дозволити виконання
chown user:group file   # change owner / змінити власника

Networking / Мережа
ip a             # show IP addresses / показати IP
ping 8.8.8.8     # test connection / перевірити з’єднання

Package Management / Керування пакетами
sudo apt update         # update repo info / оновлення репозиторіїв
sudo apt install nmap   # install package / встановити пакет

 File Search / Пошук файлів
 find / -name file.txt 2>/dev/null   # search file by name / пошук за назвою
