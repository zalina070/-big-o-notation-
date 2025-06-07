# -big-o-notation-
// Функция 1: Выводит "Hello" numberOfTimes раз
function sayHello(numberOfTimes) {
  // Время: цикл выполняется numberOfTimes раз => O(n)
  // Память: использует только переменную i и строку, память не зависит от n => O(1)
  for (var i = 0; i < numberOfTimes; i++) {
    console.log("Hello");
  }
}

// Функция 2: Выводит произведения num1 * num2 для всех num1 и num2 от 1 до n
function logMultiples(n) {
  // Время: два вложенных цикла по n => O(n^2)
  // Память: константная, используются счетчики num1 и num2 => O(1)
  for (var num1 = 1; num1 <= n; num1++) {
    for (var num2 = 1; num2 <= n; num2++) {
      console.log(num1 * num2);
    }
  }
}

// Функция 3: Выводит "test" для каждой комбинации num1 от 1 до a и num2 от 1 до b
function testFunction(a, b) {
  // Время: вложенный цикл a * b => O(a * b)
  // Память: только счетчики, не зависит от a и b => O(1)
  for (var num1 = 1; num1 <= a; num1++) {
    for (let num2 = 1; num2 <= b; num2++) {
      console.log("test");
    }
  }
}

// Функция 4: Выводит "test" x раз
function sum(x) {
  // Время: цикл от 0 до x => O(x)
  // Память: только счетчик i => O(1)
  for(let i = 0; i < x; i++) {
    console.log("test");
  }
}

// Функция 5: (пример) Выводит все пары (i, j) для i и j от 0 до n-1
function printPairs(n) {
  // Время: вложенный цикл n * n => O(n^2)
  // Память: константная, используются счетчики i и j => O(1)
  for (let i = 0; i < n; i++) {
    for (let j = 0; j < n; j++) {
      console.log(i, j);
    }
  }
}
