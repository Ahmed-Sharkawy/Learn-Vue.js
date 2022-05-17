# Learn-Vue.

## محتوا الكورس
#####  الفيديو الاول
- وما الهدف من الكوس vue.js الفيديو الاول من الكوس مقدمة عن

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

#####  الفيديو التاسع و العاشر
- v-if="condition" وظيفتة تحديد شرط
- v-else-if="condition" وظيفتة تحديد شرط ثاني لو لم يتحقق الشرط الاول
- v-else وظيفتة تحديد شرط الاخير لو لم يتحقق اي شرط
- v-once وظيفتة عدم تحديث العنصر عند التحديث
- v-show="value" وظيفتة بصناعة العنصر ولاكن لايظهر الي إذا كان القيمة موجودة

```js
  <p v-if=" age < 18 ">You are not over the legal age</p>
  <p v-else-if=" age >= 40 ">You are over the required age</p>
  <p v-else> you Didnt Set A  Name</p>
  <p v-once> you Didnt Set A Name</p>
  <p v-show="name"> you Didnt Set A Name</p>
```

#####  الفيديو الحادي عشر و الثاني عشر

- v-bind:attribut فقط attribut وظيفتها نعمل مع
- v-on: وتتحكم في ماذا يفعل عند الضغط علية Events تتعامل مع العناصر
- v-model: وتتغير دينمك يمكن صنع شرط من حلالها value و input فقط وتقوم بعمل ربط بين attribut وظيفتها نعمل مع

```js
  <a :href="url">
    <img v-bind:src="urlImage" alt="" srcset="">
  </a>
  <p> Counter Is {{ counter }}</p>
  <button v-on:click.once="counter++">button</button>
```

#####  الفيديو الثالث عشر

