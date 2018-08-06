# Переделать тесты на describe, it

# Убрать возврат dummyValue из findShorthandValue (поискать кейсы в n1/webapp)
## invalid cases
```js
// Непонятно зачем мы экспортим экшены, но сейчас такой кейс не обрабатывается
export const actions = {
   // ...
};

const store = {
    actions
}
```


## + valid cases
```js
// ТАкие кейсы мы не можем обрабатывать, просто скипаем
import actions from '..';
```
```js
// Скипаем:
{
    actions: {

        ...createActions(['creditPeriod', 'interestRate', 'phone']),
    }
}
```


# Добавить eslint + prettier

# Добавить CI