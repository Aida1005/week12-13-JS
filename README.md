# week12-13-JS

### Вопросы 

1. Как создать дату 24 января 2021 года, 22 часа 51 минута? Временная зона — местная.
let day = new Date(2021,0,24,22,51);
    console.log (date);

2. Для чего предназначен метод `getDay()`?
День недели.Причем, воскресенье - это день номер 0 , понедельник - 1 и тд.

3. Как посчитать, сколько секунд осталось до завтра?
function getSecondsToTomorrow() {
  let now = new Date();
  let hour = now.getHours();
  let minutes = now.getMinutes();
  let seconds = now.getSeconds();
  let totalSecondsToday = (hour * 60 + minutes) * 60 + seconds;
  let totalSecondsInADay = 86400;

  return totalSecondsInADay - totalSecondsToday;
}

4. Для чего предназначен метод `getDate()`?
Метод getDate() возвращает день месяца указанной даты по местному времени.

5. Что выведет `console.log(d)` ?
let d = new Date(2016, 2, 9);

console.log(d);//Wed Mar 09 2016 00:00:00

6. Что делает `getTimezoneOffset()` ?
Метод getTimezoneOffset() возвращает разницу в минутах между датой, оцененной в часовом поясе UTC, и той же датой, оцененной в местном часовом поясе.

7. Что выведет консоль?
let date = new Date();
console.log(date.getUTCHours());//12

8. Для чего предназначен метод `getHours()` объекта Date?
Метод getHours() возвращает часы указанной даты по местному времени.

9. Что выведет консоль?

let d = new Date(); 
let y =  d.getFullYear();
console.log(y);//2023

10. В чём ошибка в коде?

    let y = new Date(); 
    let d = y.getDate();
    console.log(d);//16
    
    

