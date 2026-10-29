cd lab-1
venv\Scripts\activate
python manage.py runserver - запуск сервера
docker compose up -d - поднимаем базу 

Получить одного сотрудника по id, обновить и удалить:
curl http://127.0.0.1:8000/api/employees/1/
curl -X PATCH http://127.0.0.1:8000/api/employees/1/ -H "Content-Type: application/json" -d '{"position": "Ведущий менеджер"}'
curl -X DELETE http://127.0.0.1:8000/api/employees/2/

http://127.0.0.1:8000/api/employees/
