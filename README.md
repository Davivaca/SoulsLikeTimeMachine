# SoulsLikeTimeMachine

## About the game

## My process of making this game

### First class I attended

https://youtu.be/KnfQo32ME5g

First create your initial sprite and change the image from 64x64 to 16x16

Inside the objects folder create an object for the player sprite you made.

In rooms you can place objects in instances.

Now starting to code, first in the player object you need to create a create event.

After editing the room it is recommended that you enable and edit the first camera.

The code step so far 
```
right_key = keyboard_check(vk_right);
left_key = keyboard_check(vk_left);
up_key = keyboard_check(vk_up);
down_key = keyboard_check(vk_down);

xspd = (right_key - left_key) * move_spd;
yspd = (down_key - up_key) * move_spd;

// Colision part

if place_meeting(x + xspd, y, obj_wall) == true
{
xspd = 0;
}
if place_meeting(x, y + yspd, obj_wall) == true
{
yspd = 0;
}

x += xspd;
y += yspd;
```

keyboard_check is a very important function where you use it to make the computer keys do something.

## Programming issues

### Magic formula

```
git checkout master   
git branch main master -f    
git checkout main  
git push origin main -f 
```
