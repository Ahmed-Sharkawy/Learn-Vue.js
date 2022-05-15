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

#####  الفيديو السابع و الثامن
- v-text="" [text] وظيفتها ادخال بيانت داخل العنصل من النوع
- v-html="" [Element HTML] وظيفتها تقوم ب ادخال بيانات او تقوم ب انشاء عنصر جديد elemnt
- v-for="" تقوم بعمل لوب علي العناصل عن طريق اعطاع اول متغير من علي اليسار والمتغير الذي يحمل الداتا علي اليمين وبينهم in

```js
  <p v-text=" name ? name : 'No Name'"></p>
  <p v-html="title"></p>
  <ul>
    <li v-for="skill in skills">
      {{ skill }}
    </li>
  </ul>
  <ul>
    <li v-for="(skill, index) in skills">
      {{ index }} => {{ skill }}
    </li>
  </ul>
  <ul>
    <li v-for="(test, index) in completedTest">
      {{ index }} => {{ test.testName }} || {{ test.testResult }}
    </li>
  </ul>
```