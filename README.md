# SCSS Function Fluid

A package for integrating function to create responsive typography and design.

![npm](https://img.shields.io/npm/v/@bu0nq/scss-function-fluid?style=for-the-badge)
![npm](https://img.shields.io/npm/dt/@bu0nq/scss-function-fluid?style=for-the-badge)

Documentation: [EN](README.md) | [RU](README.RU.md)

___

## Installation

You can install the package automatically using NPM:

```
npm i @bu0nq/scss-function-fluid
```

## Usage

To use the package, import it into your project:

```scss
@use "@bu0nq/scss-function-fluid" as *;

.demo {
    font-size: fluid(16px, 24px);
}
```

## Changing the namespace

You can change the namespace during function import and use the function with a different namespace:

```scss
@use "@bu0nq/scss-function-fluid" as function;

.demo {
    font-size: function.fluid(16px, 24px);
}
```

## Changing the variables

You can redefine the default values for the specified variables when importing the function:

```scss
@use "@bu0nq/scss-function-fluid" as * with (
    $min-breakpoint: 480px,
    $max-breakpoint: 1536px,
    $unit: vw,
);
```
