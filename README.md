```javascript

for ( var = i; i < myArray.length; i++) {
   //   выполнить какие-то операции над  myArray[i]
   //   при каждой итерации выясняется длинна массива
   //   особенно если myarray является не массивом, а объектом HTMLCollection.
   //   HTMLCollection – это объект, возвращаемый методами DOM, такими как:
   //   document.getElementsByName()
   //   document.getElementsByClassName()
   //   Именно поэтому при работе с циклами for лучше определять длину массива заранее
};
    for ( var = i; max = myArray.length; max < i; i++) {
       //   При таком подходе значение свойства length будет извлекаться всего
       //    один раз за все время работы цикла.
};


//   Get Pseudo-Element Properties with JavaScript
    
    // Get the color value of .element:before
       var color = window.getComputedStyle(
	       document.querySelector('.element'), ':before'
       ).getPropertyValue('color');

    // Get the content value of .element:before
            var content = window.getComputedStyle(
	        document.querySelector('.element'), ':before'
       ).getPropertyValue('content');        
    

// CSS: User Agent Selectors

<html>
    <head> … </head>    
    <body>
        <script>
            var b = document.documentElement;
              b.setAttribute('data-useragent',  navigator.userAgent);
              b.setAttribute('data-platform', navigator.platform );
              b.className += ((!!('ontouchstart' in window) || !!('onmsgesturechange' in window))?' touch':'');
        </script>
        …
    </body>
</html>

//output like this:

<html 
    data-useragent='Mozilla/5.0 (Macintosh; Intel Mac OS X 10_6_8) AppleWebKit/535.1 (KHTML, like Gecko) Chrome/13.0.782.112 Safari/535.1' 
    data-platform='MacIntel'>
    
//How use:

html[data-useragent*='Chrome/13.0'] .nav{
    background: tomato // or something like this
}

// For different platform
html[data-useragent*='Chrome/13.0'][data-platform='Win32']

//you may have noticed the "touch" class on touch devices
.touch li .action{
    opacity:1;
}




