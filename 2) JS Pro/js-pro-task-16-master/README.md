# Практическое задание

Реализуйте и экспортируйте по умолчанию функцию, которая принимает на вход один аргумент - путь до директории и подсчитывает общий размер всех файлов внутри нее. Необходимо подсчитывать только размер файлов, директории должны быть игнорированны.

Функция должна возвращать промис, готовый к использованию.

Например:

```js
import getFilesSize from './src';

getFilesSize('./example')
  .then((totalSize) => {
    console.log(totalSize);
  });
// 256
```

**Подсказки:**
1. Используйте `promise` версии методов `fs`;
