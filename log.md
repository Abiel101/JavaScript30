[09.28.2022]
# JAVASCRIPT DRUM KIT > Moving to Notion
- Adding event listener for a keydown because we are trying to get what key it is and we can see the keycode property.
- The same way we are able to grab attribute using css we can do the same in javascript

 `const audio = document.querySelector('audio[data-key=65]')` 

which I think is super cool but what makes it even cooler is that we can go further and select the keycode of the event it self at the same time. 

`const audio = document.querySelector(`audio[data-key="${e.keyCode}"]`)` (dont forget to make sure you add the correct spelling camale case)

    This is amazing because I am able to get the property of this variable too by using ES6 template strings ${}

This over all saves time and effort in having to create classes or ID I can just select using attributes especially if these things are not connected together by ID I can use there attributres if they have any.

Play audio elements in HTML javascript wont play it again because to javascript itll already be playing we need to make it so that it plays it again when we let go of the key or stops when we let go of the key.

With query selector depedning which one you are trying to select, if you want to select all you use `querySelectorAll` if only one `querySelector` and then you specify that only getting one or all.
The reason why we are not able to use an event listener when setting up when to end the animation is because as what wes said "When you have a Node list of elements, you can not listen on all of them at the same time, you have to go one at a time" hints `forEach()`.

```
keys.forEach(key => key.addEventListener('transitionend', removeTransition));

```
In this code we are saying forEach, key add event listener "transitionend" and run the function removeTransition.

> Something intersting that I found is that Wes uses a lot of console.log to see what kind of information he is given and then uses that information to be able to solve the piece of code he is targetting. Super smart.


## Question
1. Why are you able to do this ```if(!audio) return;``` and for it to work?
2. What function do you use to be able to play audio in HTML using JS?
3. what does `.currentTime` do when you use it?
4. What does forEach() do in javascript?
5. What does the "transitionend" event listener do?

