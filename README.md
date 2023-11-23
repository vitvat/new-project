#Створіть в своєму середовищі новий каталог з назвою "new-project".
mkdir new-project

#Перейдіть до каталогу "new-project".
cd new-project

#Ініціалізуйте новий публічний Git-репозиторій всередині каталогу "new-project".
git init

#Створіть новий файл з назвою "README.md" і додайте до нього початковий текст.
touch README.md
vim README.md

#Підготуйте файл "README.md" до коміту.
git add README.md

#Закомітьте зміни у репозиторій з коміт повідомленням “init”.
git commit -m "init"

#Створіть нову гілку з назвою "development" і перейдіть до неї.
git branch development
git checkout development

#Додайте інструкцію до файлу "README.md" і підготуйте їх до коміту.
vim README.md
git add README.md

#Закомітьте зміни у гілці "development" з повідомленням про коміт.
git commit -m "Add instructions to README"

#Об'єднайте зміни з гілки "development" у гілку "main".
git checkout main
git merge development

#Перевірте статус, переконайтеся, що все актуально.
git status

#Закомітьте зміни
git commit -m "Merge changes from development to main"

