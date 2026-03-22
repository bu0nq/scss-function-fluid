# SCSS Function Fluid

Пакет для интеграции функции для создания адаптивной типографики и дизайна.

Документация: [EN](README.md) | [RU](README.RU.md)

___

## Установка

Вы можете установить пакет автоматически с помощью NPM:

```
npm i @bu0nq/scss-function-fluid
```

## Использование

Чтобы использовать этот пакет, импортируйте его в свой проект:

```scss
@use "@bu0nq/scss-function-fluid" as *;

.demo {
    font-size: fluid(16px, 24px);
}
```

## Изменение пространства имен

Вы можете изменить пространство имен во время импорта функции и использовать функцию с другим пространством имен:

```scss
@use "@bu0nq/scss-function-fluid" as function;

.demo {
    font-size: function.fluid(16px, 24px);
}
```

## Изменение переменных

Вы можете переопределить значения по умолчанию для указанных переменных при импорте функции:

```scss
@use "@bu0nq/scss-function-fluid" as * with (
    $min-breakpoint: 480px,
    $max-breakpoint: 1536px,
    $unit: vw,
);
```
