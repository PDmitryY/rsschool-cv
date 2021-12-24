# Dmitry Petrochenkov


**Contact imformation:**
- Phone: +375 29 3901653
- E-mail: p.dmitry.y@gmail.com
- GitHub: PDmitryY

**About Myself:**

I have been working in the auto business for over 14 years. 2 times passed the way from an ordinary employee to the head of the department. Now I am planning to change my occupation. For myself, I chose the path of a software developer in front-end development. I want to work in a rapidly developing field among a young team that will motivate me to constant self-development. I consider my strong features to be good communication skills, dedication, stress resistance, positive attitude to life. Of the negative traits I can name obstinacy and love of freedom and a constant desire to do more and better than required.

**Skills:**
- HTML 5
- CSS 3 (Framework Bootstrap, Preprocessor SCSS, BEM methodology).
- JavaScript (Fundamentals,Functional Programming, OOP, Asynchronous JavaScript, ES5, ES6+, DOM), jQuery.
- React JS.
- JSON.
- Python (basic knowledge) - Django Framework (basic knowledge).
- PHP (basic knowledge).
- Version control: Git (remote services: GitHub, GitLab).
- Module Bundlers: Webpack.
- SQLite (basic knowledge).
- PostgreSQL (basic knowledge).
- Figma(for web development).
- Editors: Sublime, Brackets, VSCode, PyCharm community.


**Education**
- 2002-2007 BNTU
- 2006-2007 IBT Atlant-M
- 2015 "Современный Front-End с использованием HTML5 и JavaScript" (IT-Academy Belhard)
- 2017 JavaScript/Front-End course (RSSchool)
- Online courses, services and books (https://learn.javascript.ru, CS50, Codewars, Checkio...)

**Languages:**
- Belarusian (native)
- Russian (native)
- English B1
- Ukrainian (intermediate knowledge)
- Polish (basic knowledge)
- German (basic knowledge)

**Code example:**

Function Cache KATA from CODEWARS: *If you are calculating complex things or execute time-consuming API calls, you sometimes want to cache the results. In this case we want you to create a function wrapper, which takes a function and caches its results depending on the arguments, that were applied to the function.*

```
function cache(func) {
  let cache = [];
  
  let arrEqual = function(a, b){
    if(!Array.isArray(a) || !Array.isArray(b)){return false;}
    if(a.length !== b.length){return false;}
    for (let i = 0; i < a.length; i++){
      if(a[i] !== b[i]) {return false;}
    }
    return true;
  };
  
  let inCache = function(args){
    let data = 'blalblablallfffffffffffffffffffffffffffffffffffffff';
    cache.forEach(function(val, i, arr){
      if(arrEqual(val[0],args)){
        data = val[1];
      }
    });

    return data;
  };
  
  return function(){
    if(!func){return undefined;};
    
    let args = Array.prototype.slice.call(arguments);
    
    let cacheResults = inCache(args);
    if(cacheResults !== 'blalblablallfffffffffffffffffffffffffffffffffffffff') return cacheResults;
    
    let res = func.apply(this, args);
    cache.push([args, res]);
    return res;
  }
}

```

**My projects** 

- https://pdmitryy.github.io/PDmitryY.game.github.io/
- https://pdmitryy.github.io/youtube/