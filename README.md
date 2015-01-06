JavaScript patterns && tricks
===================

#### Циклы for

```javascript

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


#### Get Pseudo-Element Properties with JavaScript
    
    // Get the color value of .element:before
       var color = window.getComputedStyle(
	       document.querySelector('.element'), ':before'
       ).getPropertyValue('color');

    // Get the content value of .element:before
            var content = window.getComputedStyle(
	        document.querySelector('.element'), ':before'
       ).getPropertyValue('content');        
    
