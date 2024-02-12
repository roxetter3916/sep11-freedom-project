# Entry 3
##### 2/5/24
Up untill now the last month up I've been working on going more in depth for learning my tool to be able to understand it more clearly for the development of my game. As of now I've been focusing on creating entities and some music/graphics. The first area I tackled was being able to create entities.

### Entities
I've realized that in order to fully understand how impact works I have to get a layout of the building blocks for it. Entities represent almost anything, from objects to characters. Anything ranging from the actual player to items.

```
ig.module(
    'game.entities.roxette'
)
.requires(
    'impact.entity'
)
.defines(function(){

    var Roxette = ig.Entity.extend({

        size: {x: 32, y: 32}


        init: function(x, y, settings) {
            this.parent(x, y, settings);
            this.addAnim('idle', 1, [0]);
            this.addAnim('run', 0.07, [1, 2, 3, 4, 5, 6]);
        },
```
Since I didn't wanna confuse myself, I only started with a simple idle animation and a running one. The `1`, represents the speed of the animation while the `[0]` is an array that shows frames. 

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)