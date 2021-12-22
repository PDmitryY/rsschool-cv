[rsschool-cv](https://PDmitryY.github.io/rsschool-cv/)

#Dmitry Petrochenkov


**Contact imformation:**
- Phone: +375 29 3901653
- E-mail: p.dmitry.y@gmail.com
- GitHub: PDmitryY


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
- 2015 Front-End course (IT Academy)
- 2017 Front-End course (RSSchool)

**Languages:**
- Belarusian (native)
- Russian (native)
- English B1
- Ukrainian (intermediate knowledge)
- Polish (basic knowledge)
- German (basic knowledge)

**Code example:**

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