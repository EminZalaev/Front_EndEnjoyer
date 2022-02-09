#Устанавливаем python и pip

python3 --version //Проверяем

Если не установлен

1.1 sudo apt install python3 //Устанавливаем

pip3 --version //Проверяем

Если не установлен

1.1 sudo apt -y install python3-pip //Устанавливаем

#Создаём и настраиваем среду

python3 -m venv venv //Создаём
source venv/bin/activate //Активируем
pip install --upgrade pip // Обновляем pip
pip install -r requarements.txt // Устанавливаем пакеты для работы нашего приложения
#Запускаем приложение(из под виртуального окружения)

source venv/bin/activate //Заходим в созданное ранее виртуальное окружение
python manage.py makemigrations //Создаём миграции
python manage.py migrate //Проводим миграции
python manage.py runserver //приложение запущенно на 8000 порту

