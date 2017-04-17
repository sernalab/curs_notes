# CURSE NOTES WEEK 1

## DAY ONE

#### CONSOLE

`-rm -rf` it remove all folder and files

#### ABOUT MARKDOWN

- [Shortcut Markdown](https://github.com/SublimeText-Markdown/MarkdownEditing) 

- [Learning Markdon](https://blog.ghost.org/markdown/)

- [Markdown Basics](http://rmarkdown.rstudio.com/authoring_basics.html)

#### ABOUT GITHUB

- Use `git status` to see our status project (if our files are tracked or untracked)
- Use `git log` to see author, date and commit number
- Use `git log --stat` to see changes
- Use `git config -l` it show your conf (user.name, user.email...)
- Use `git add .` or `git add --all` to add all files in stage area
- Use `git push -u origin master`to push your local repository to remote one

__HOW TO USE GIT (LOCAL)__

- Use `git init` to initialize repository --> (repository is a hidden folder, if u remove the folder u can't use git)
- Use `git add` to add file in Staging Area
- Use `git commit -m` followed by a message ("first commit") 

__HOW TO USE GIT (REMOTE)__

- `git init`
- `git remote add origin URL` 
- Use `git commit -m` 
------

![LOCAL GIT](http://i.imgur.com/DDPtmnD.png)

------




## DAY TWO

#### MORE GITHUB

**Some commands:**

- `git log --stat` to see what changed and what we added
- `git checkout` restore working tree files
- `git remote -v` to see if is connected our local repository
- `git clone` take a remote repository and create a folder
- `git add` '*.txt' it add all files .txt

------------------------------
#### STARTING THE ~~FANTASTIC~~ WORLD OF JAVASCRIPT
------------------------------

No objects: 
```
Number
String
Boolean
Undefined
Null
```

Objects:
```
functions
arrays
object
```

Modules are usefull to compare even or odd (par o impar)

```javascript
var res = '\n';
for (var i=1; i<=10; i++){
    for(var j=1; j<=10; j++){
        res += i*j + '\t';
    }
    res += '\n';
}
```


## DAY THREE

__FUNCTIONS__

[Parts of functions](https://github.com/juanmaguitar/javascript-notes/tree/master/markdown-en/04-functions)

[Parameters](https://github.com/juanmaguitar/javascript-notes/tree/master/markdown-en/04-functions#parameters) 

[Callback functions](https://github.com/juanmaguitar/javascript-notes/tree/master/markdown-en/04-functions#callback-functions)

[Closures](https://github.com/juanmaguitar/javascript-notes/tree/master/markdown-en/04-functions#closures)

[Lexical scope](https://medium.com/@nickbalestra/javascripts-lexical-scope-hoisting-and-closures-without-mystery-c2324681d4be)

"When we pass a function A as an argument of another function B and B executes A, we tell that A is a callback function"

```javascript
>>> function invoke_and_add(a, b){ return a() + b(); }
>>> function one() { return 1; }
>>> function two() { return 2; }
>>> invoke_and_add(one, two);
>3
>>> invoke_and_add(one, function(){return 7;})
>8
```


Closure example:
```javascript
function timesCallFn() {
  var times = 1;
  return function() {
    return times++;
  }
};

var m = timesCallFn();
```



### ARRAYS

[Methods](https://github.com/juanmaguitar/javascript-notes/tree/master/markdown-en/06-global-objects/arrays#basic-methods-of-array)

__HOW__ to creat an object

1.
```javascript
var hero = {
  breed: 'Turtle',
  occupation: 'Ninja'
};
```
2.
```javascript
var hero = {};
hero.breed = 'Turtle';
hero.name = 'Leonardo';
```
3.
```javascript
function createHero() {
  return {
    breed: 'Turtle',
    occupation: 'Ninja'
  }
}
var hero = createHero();
```
4.
```javascript
function createHero(customName, customOccupation) {
  return {
    breed: customName,
    occupation: customOccupation
  }
}
var hero = createHero('Turtle', 'Ninja');
var hero = createHero('Power', 'Ranger');
```
5.__Constructor function__
```javascript
function Hero(name) {
  this.name = name;
  this.occupation = 'Ninja';
  this.whoAreYou = function() {
    return "I'm " + this.name + " and I'm a " + this.occupation;
  }
}

var h1 = new Hero('Michelangelo');
var h2 = new Hero('Donatello');
```


## DAY FOUR

[Regular expressions](https://github.com/juanmaguitar/javascript-notes/tree/master/markdown-en/08-regular-expressions#regular-expressions)

[Some examples from @juanmaguitar:](https://github.com/sernalab/javascript_exercises/tree/master/higher_order_functions_examples) 


Funciones constructoras:
array
function
object
var myArray - new Array(2,4,5)











