---
layout: post
title: "Radians"
date: 2023-05-02 14:39:11 +0200
image: https://i.pinimg.com/originals/80/c3/4c/80c34c5cb6ca068f950fbe2df641d940.gif
---
Radians are a thing that will be used throughout all of these tutorials. If you're afraid you don't have a 100% grasp on what they are, make sure to read ahead.

Radians are a way of measuring angles, much like degrees (which you may be more used to). Degrees divide a circle into 360 part, each part being 1 degree. Radians divide a circle not in 360 parts, but in 2π parts, which is approximately 6,28.

If you're not familiar with π, it's the value you get when you divide the circumference of a circle by its diameter. It's a number used all throughout math in anything that has to do with circles (and more).

Most (if not all) math related functions in programming expect you to use radians. It's technically possible to convert from degrees to radians whenever needed, but you can avoid a lot of headaches when you know about the numbers you're working with.

Enough talk, let's get some visuals! For these examples, we'll use a unit circle, which is nothing more than a circle with a radius of 1. As stated earlier, a full circle is 2π radians (≈ 6.28). That being said, how much would half a circle be then?

$$ \dfrac{2π}{2} = π $$

<div style="display: flex">
  <div style="flex: 1; text-align: center">
    Yes, only π! That looks like:
    <img src="https://i.imgur.com/lUA6mzS.png"
      alt="π radians"
      style="display: block; width: min(100%, 300px); height: auto; margin: 8px auto;"
    />
  </div>
  <div style="flex: 1; text-align: center">
    And then, 1 radians look like this:
    <img src="https://i.imgur.com/hg2ZD6i.png"
        alt="1 radians"
        style="display: block; width: min(100%, 300px); height: auto; margin: 8px auto;"
    />
  </div>
</div>

If you prefer some more visuals, I recommend watching [this](https://www.youtube.com/watch?v=ifBhTdsTMuE) short video to get a better understanding.

## Converting from and to radians

Now that you know what radians are, it's good to know how to convert to and from them when you have degrees. It's good to try and always work with radians, but sometimes you can't avoid working with degrees, or it simply becomes more readable by doing so.

Converting is pretty straight forward. A full circle in degrees is 360 and 2π in radians. That means that 180 degrees must equal π.

If we work this into a formula, we can deduce we need to divide our amount of degrees by 180, and then multiply it by π. If we do that, we get:

$$ \dfrac{degrees}{180} \times π = radians $$

Using this formula, we can convert degrees into radians. In Java, you don't have to write this formula our yourself, you can just use [Math.toRadians(double)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Math.html#toRadians(double)).

Then, converting from radians to degrees. For this, we must invert the formula we created earlier. So we first divide by π, and then multiply by 180. Doing this gives us:

$$ \dfrac{radians}{π} \times 180 = degrees $$

Again, you probably won't have to write this formula out in code yourself either, it's a lot better to just use [Math.toDegrees(double)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Math.html#toDegrees(double)).

There you go! You now know about the basics of radians, which you will need in all further tutorials. There's nothing fancy we can do with just radians unfortunately, but all great things start small. The next tutorial is about drawing circles, you can find it [here](circles)!