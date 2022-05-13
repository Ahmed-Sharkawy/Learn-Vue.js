# Learn-Vue.

## محتوا الكورس
#####  الفيديو الاول
-  الفيديو الاول من الكوس مقدمة عن وما الهدف من الكوس vue.js.

##### الفيديو الثاني
- Create project Vue.js.
- install Vue.js => version[2].
- extensions vue.js.

##### االفيديو الثالث
- Single Page Application شرح المعني واية الغرض و لية المصطلح دا موجود
- MVC ما هوا وما الفرق بين MVVM Vue.js

##### االفيديو الرابع
- انشاء object js حتا اتمكن من التحكم في عناصر HTML واضافة عناصة والتعديل علي العناصر
```js
<div id="app">
  <p>Welcome {{ 'Dev ' + name }} We Are Happy to see you.</p>
  <p>Your age is: {{ age + ' Years'}} </p>
</div>

<script>
var app = new Vue({
  el: '#app',
  data: {
    name: 'Ahmed Al Sharkawy',
    age: 22,
  }
})
</script>
```

##### الفيديو الخامس و السادس
- استكمال صنع array من objet & methode
```js
skills: ['Html', 'Css', 'PhP'],
completedTest: [
     {
        testNmae: 'first Test',
        testResult: '80%'
      },
     {
        testNmae: 'Second Test',
        testResult: '70%'
     },
],
methods: {
    ShowNewDate: function () {
      this.date = Date()
},
```