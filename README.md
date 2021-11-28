# AT-27-Multi
Сычев Тимофей
IO-bound. Проверяем ссылки на страницах Википедии
Синхроонная обработка ссылок заняла 1453 секунды  
![image](https://user-images.githubusercontent.com/72296553/143772853-5d352528-5d56-4ac7-8c2a-72bd8deeec74.png)  
Асинхронная обработка при 5 воркерах 285 секунд. Оперативная память была загружена почти на максимум, процессор не более чем на 20%, нагрузка на сеть была не самая значительная  
![image](https://user-images.githubusercontent.com/72296553/143775182-54cd8a72-ae27-4b2a-aad1-f9ec9c3426f1.png)  
![image](https://user-images.githubusercontent.com/72296553/143775194-60d9afb0-b1f9-4b45-b72e-b253868eb72e.png)  
Асинхронная обработка при 5 воркерах 142 секунды. Оперативная память была загружена почти на максимум, процессор не более чем на 60%, нагрузка на сееть выросла значительно по сравнению с 5 воркерами  
![image](https://user-images.githubusercontent.com/72296553/143775240-26b25f77-b53d-477d-bd19-67a0a99f0d38.png)  
![image](https://user-images.githubusercontent.com/72296553/143775252-e8f4c41e-0ec0-41cf-959d-baf9794fe126.png)  
![image](https://user-images.githubusercontent.com/72296553/143775258-02617e72-a49e-4ff7-9d94-28c3e59d2c33.png)  
Асинхронная обработка при 100 воркерах 23 секунды. Оперативная память была загружена почти на максимум, процессор 100%, загрузка сети было очень значчиельно, выросла в несколько раз  
![image](https://user-images.githubusercontent.com/72296553/143775377-2e740a62-a502-4a6f-af36-5f572ac9a872.png)  
![image](https://user-images.githubusercontent.com/72296553/143775388-9503664f-b82b-47ef-b545-7c9fce5c292a.png  
![image](https://user-images.githubusercontent.com/72296553/143775400-566e0d25-c95a-4edd-814f-52f9d5c6f8ea.png)  
CPU-bound. Генерируем монетки  
На одном ядре генерации одной монеты заняла 14 секунд   
![image](https://user-images.githubusercontent.com/72296553/143775873-9b93e2a4-2b01-4544-9210-9580a9643bd9.png)    
При использовании ProcessPoolExecutor при 2 воркерах генерации одной монеты заняла 28 секунд, процессор нагружался на 30-35%, оперативная память была загружена почти на максимум, сеть практически не нагружена  
![image](https://user-images.githubusercontent.com/72296553/143777142-a23248e1-071a-4370-be70-85c9da802ea3.png)  
![image](https://user-images.githubusercontent.com/72296553/143777315-55ad5e09-2c4b-42a8-a822-019a66f78fd3.png)  
При использовании ProcessPoolExecutor при 4 воркерах генерации одной монеты заняла 46 секунд, процессор нагружался на 30-35%, оперативная память была загружена почти на максимум, сеть практически не нагружена   
![image](https://user-images.githubusercontent.com/72296553/143777351-638f5a69-8ee2-4bb0-a112-99d225594841.png)   
![image](https://user-images.githubusercontent.com/72296553/143777356-d922e2cf-b271-48bf-84ab-31504895e048.png)    
При использовании ProcessPoolExecutor при 5 воркерах генерации одной монеты заняла 76 секунд, процессор нагружался на 30-45%, оперативная память была загружена почти на максимум, сеть практически не нагружена   
![image](https://user-images.githubusercontent.com/72296553/143777378-38a56b8b-209f-47d3-860c-83342a6706ac.png)   
![image](https://user-images.githubusercontent.com/72296553/143777395-fd4fc925-0123-4cfc-9f51-163d83eb120e.png)   
При использовании ProcessPoolExecutor при 10 воркерах генерации одной монеты заняла 35 секунд, процессор нагружался на 30-35%, оперативная память была загружена почти на максимум, сеть практически не нагружена   
![image](https://user-images.githubusercontent.com/72296553/143777408-50ae39d6-a11c-428c-ab23-1272a88c3a91.png)   
![image](https://user-images.githubusercontent.com/72296553/143777418-0f693a10-7551-48aa-9ac8-58f9d35ba691.png)   
При использовании ProcessPoolExecutor при 100 воркерах выдалась ошибка   
![image](https://user-images.githubusercontent.com/72296553/143777447-6d27881b-26d3-4d2b-a67f-3891fa0f86ab.png)   
При использовании ProcessPoolExecutor при 61 воркерах генерации одной монеты заняла 60 секунд, процессор нагружался на 30-35%, оперативная память была загружена почти на максимум, сеть практически не нагружена  
![image](https://user-images.githubusercontent.com/72296553/143777478-704f8c47-779b-4e62-807e-2a8d8857fe9b.png)   
![image](https://user-images.githubusercontent.com/72296553/143777488-0862e55b-d160-4f52-94a9-330af0d0e993.png)   

