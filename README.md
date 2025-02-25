# CuteCat - площадка для размещения своих любимых животных

[![Main Kitty workflow](https://github.com/shft1/kittygram_final/actions/workflows/main.yml/badge.svg)](https://github.com/shft1/kittygram_final/actions/workflows/main.yml)

<img width="884" alt="image" src="https://github.com/user-attachments/assets/c03243e5-801a-4c25-8803-dc2744216e32" />

---

### Стек технологий:
Python, Django REST Framework, Docker, Docker Compose, SQLite, PostgreSQL, Nginx, GitHub Actions, React

---

### Инструкция по развертыванию:
**Клонируйте репозиторий:**

```
git clone git@github.com:shft1/CuteCat.git
```

**Cоздайте и активируйте виртуальное окружение:**

```
python3 -m venv venv
```

* _Если у вас Linux/macOS_

    ```
    source venv/bin/activate
    ```
* _Если у вас Windows_

    ```
    source venv/scripts/activate
    ```

**Установите зависимости из файла requirements.txt:**

```
pip install -r requirements.txt
```

**Заполните файл .env в директории `backend` :**
```
POSTGRES_DB - имя базы данных (если не указать, то БД - SQLite)
POSTGRES_USER - имя пользователя с правами к базе
POSTGRES_PASSWORD - пароль пользователя
DB_NAME - имя контейнера, в котором запущена СУБД
DB_PORT - порт, на котором работает контейнер с СУБД
SECRET_KEY - для секретного ключа
DEBUG - что включения режима отладки значение True/true
ALLOWED_HOSTS - разрешенные хосты
```

**Запустите приложение CuteCat командой:**
```
docker compose up
```

---

### Дополнительные возможности для разработчиков

Пуш в ветку main запускает CI/CD (тестирование и деплой) Kittygram, а после успешного деплоя вам приходит сообщение в телеграм.

---

### Примеры использования

**_Форма регистрации_**

<img width="627" alt="image" src="https://github.com/user-attachments/assets/054289ad-e72f-4cad-8736-36f4482e92fc" />

**_Форма создания поста_**

<img width="1210" alt="image" src="https://github.com/user-attachments/assets/b722bfa4-6206-4669-8dc3-10274080687e" />

**_Главная страница_**

<img width="1234" alt="image" src="https://github.com/user-attachments/assets/b189cbf6-b678-48ff-aa78-6570879d37d3" />

**_Страница котика_**

<img width="1217" alt="image" src="https://github.com/user-attachments/assets/c01388ad-f7e9-43e2-abef-4d0b076a9e3e" />

---

### Автор 
Алексей
[Ссылка на гитхаб](https://github.com/shft1)
