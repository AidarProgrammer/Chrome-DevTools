# Анализ производительности веб-страницы

## 📊 Вкладка Network

### 🔄 Дублирование кода
1. **advanced.4fdec4f0c66230612adf.js**
   
   ![12](https://github.com/user-attachments/assets/f15fc5ba-bb14-4192-9159-15e2cb36a12c)

2. **react-with-dom-and-polyfills.min.js**  
   ![2](https://github.com/user-attachments/assets/6e2ec410-c485-4e9f-9290-8922225a077e)

3. **vendors.chunk.bundle.js**  
   ![3](https://github.com/user-attachments/assets/35e3c33d-e5f4-4aba-9bcb-7f0ee16e14f2)

4. **watch.js**  
   ![4](https://github.com/user-attachments/assets/51794364-cd32-4d7c-806c-f20bb0275d9b)

5. **advert.gif**  
   ![5](https://github.com/user-attachments/assets/32f586f6-3e17-442f-ae83-96ae905bc57d)

6. **logo** (одинаковое содержимое под разными названиями)  
   ![6](https://github.com/user-attachments/assets/032c78ff-e285-468d-aee2-6968bc91f93c)


8. **widget-button-whatsapp-and-telegram.gif**  
 ![7](https://github.com/user-attachments/assets/05a1d6a4-9db0-4946-96fd-7b8a64359e2c)
  
9. **Повторяющиеся запросы**
   ![8](https://github.com/user-attachments/assets/62a38ea6-2baf-43ec-b85b-39615e30505e)
   ![9](https://github.com/user-attachments/assets/ced317ae-eefb-4cf2-aad5-7fdffac0881d)
   ![10](https://github.com/user-attachments/assets/4beac4a8-6e3a-4505-bc0a-d7f541cf4ec8)
   ![11](https://github.com/user-attachments/assets/0d9abd4a-9d48-43fa-b922-90752ad33cea)
   
   ![12](https://github.com/user-attachments/assets/27e6158c-1484-4e2a-8a7f-b41e2f5df21c)


### 🐢 Медленно загружающиеся ресурсы
1. **Медленная загрузка изображений несмотря на то что их вес очень маленький**  
  ![image](https://github.com/user-attachments/assets/9dac9867-4b1b-480a-94ac-54816c3ec3ad)

### 🏋️ Лишний размер ресурсов
1. **Необходимо минифицировать изображения формата webp**  
   ![13](https://github.com/user-attachments/assets/3e4b92a9-febe-4b78-8b53-99f9be0c9687)


### ⛔ Ресурсы, блокирующие загрузку
1. **Запрос обрабатывается около минуты и в это время практически не происходят другие операции**  
   ![14](https://github.com/user-attachments/assets/d3fc13d0-7f91-44e6-bd28-3e12683dc6c9)
   ![15](https://github.com/user-attachments/assets/db839207-4617-462a-ac6e-533f6a90737f)


### 🧹 Что-то еще
1. **Загружается неиспользуемое изображение**  
   ![16](https://github.com/user-attachments/assets/4355f404-f41a-4848-a62c-62dd2e6416a0)
   ![17](https://github.com/user-attachments/assets/6bacaeae-61ef-44e6-ab58-f549c3bd7aa7)

2. **У нас имеется 2 файла main.js и один из них не является нужным**  
  ```JS
    function hello() {
        console.log("Hello");
    }
```
3. **Отсутствие alt у изображений**  
   ![19](https://github.com/user-attachments/assets/b25f9ae4-6a28-44b1-a069-f21e34ea8285)

## ⚡ Performance

### 📊 Основные метрики
| Метрика | Значение |
|---------|----------|
| **FCP** | 1.3559 мс |
| **LCP** | 1.5868 мс |
| **DCL** | 2.4096 мс |

![20](https://github.com/user-attachments/assets/ff8c71f1-1d9c-4ee8-bbcc-a647b074f5d9)

![21](https://github.com/user-attachments/assets/008c8f98-5e8f-4912-92ba-8c4a2d21b047)

![22](https://github.com/user-attachments/assets/f6c9873d-5307-4165-9309-685e2aa30eea)

### 🔍 LCP элемент
  ```HTML
  <p>
   <b>Web-дизайнер</b>
  	(от англ. web – сеть, Интернет) занимается оформлением сайтов. Его главная задача – подготовить интерфейс, то есть внешний вид, интернет-сайта, сделать его максимально удобным и визуально приятным для пользователей. И хотя его работа в сфере информационных технологий, для веб-дизайнера важно наличие творческого мышления, художественного восприятия и хорошего вкуса.
  </p>
  ```



### ⏱ Время обработки документа
| Этап       | Время (ms) |
|------------|------------|
| Loading    |     103    |
| Scripting  |    1928    |
| Rendering  |     562    |
| Painting   |     156    | 

![23](https://github.com/user-attachments/assets/d08d225b-76fe-40b4-bfe8-a0e5213eceb4)

## 📉 Coverage

![24](https://github.com/user-attachments/assets/c44bf406-867c-4a61-8aa5-ae3342c25588)
![25](https://github.com/user-attachments/assets/95e55a84-c938-4aec-bec8-7f30a1ee4164)

### 📦 Неиспользуемый код
| Тип кода | Неиспользуемый объем |
|----------|----------------------|
| CSS      | ~440.5 KB            |
| JS       | ~1.64 МБ (1680 KB)   |
