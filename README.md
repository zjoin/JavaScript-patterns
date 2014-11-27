JavaScript-patterns
===================

for ( var = i; i < myArray.length; i++) {
    //   выполнить какие-то операции над  myArray[i]
    //   при каждой итерации выясняется длинна массива
    //   особенно если myarray является не массивом, а объектом HTMLCollection.
    //   HTMLCollection – это объект, возвращаемый методами DOM, такими как:
    //   document.getElementsByName()
    //   document.getElementsByClassName()
    
    //   Именно поэтому при работе с циклами for лучше определять длину массива (или коллекции) заранее
};


for ( var = i; max = myArray.length; max < i; i++) {
   //   При таком подходе значение свойства length будет извлекаться всего
  //    один раз за все время работы цикла.
};

```javascript

  1. Simple mode, it styles document scrollbar:
  $(document).ready(
    function() {  
      $("html").niceScroll();
    }
  );
