# vue component life cycle demo

## Structure
```html
<header>
  <nav>
  </nav>
</header>
```

## Orders
1. beforeCreate header
1. created header
1. beforeMount header
1. beforeCreate nav
1. created nav
1. beforeMount nav
1. mounted nav
1. mounted header
1. beforeDestroy header
1. beforeDestroy nav
1. destroyed nav
1. destroyed header

## Project setup
1. `git clone`
1. `npm i`
1. `npm run serve`

## Reference
- [The Vue Instance: Lifecycle Diagram](https://vuejs.org/v2/guide/instance.html#Lifecycle-Diagram)
- [重新認識Vue.js：1-7 元件的生命週期與更新機制](https://book.vue.tw/CH1/1-7-lifecycle.html)