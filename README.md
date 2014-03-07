Leap Scroll plugin

In order to get a plugin working do the following:

- Go to the settings tab of the drop down ( upper right )

![Settings](http://i.imgur.com/4CXRX13.png)

- Click on the extensions tab ( upper left )
- Enable Developer mode ( upper right )
- Click Load upacked extension ( upper right )
- Load this folder
- Make sure that any time you make a change to the extension you reload on the extensions page!

icohen@leapmotion.com for more questions.

You will see that on any page you visit, there is a small GUI of sliders.

The parameters ( currently ) are as follows:

- Force Ratio: this will tell you how powerful your swipes are. Set it very low to slowly push the page, and high to quickly move it.
- Match Power: One of the basic mechanics of this interaction is that finger directions need to match hand directions. This means that if your hands are curled, it wont affect the scrolling at all. Changing this number will change the following function: <code> var matchPower = Math.pow( match , matchPower ); </code> What this means is that the higher this number is, the quicker the fall off will be for your fingers matching your hand.
- Match Cutoff: Whereas Match Power is a 'fade out' affect for not affecting swipes, Match Cutoff is a hard stop for swipe affecting. For instance, if Match Cutoff is at 1, swipes will NEVER affect the scrolling.

- Pinch Cutoff: The other part of this interface is a pinch interaction, where you grab and move the page to scroll. the pinch cutoff is the hard cutoff for when you are considering to be pinching. To never pinch make this 1.
- Pinch Movement Ratio: this is the amount you will move the page up and down when you are pinching

- Dampening: This is how much the speed will be multiplied every frame to gradually slow it down


Important Settings: To Just use Swipe, set Pinch Cutoff to 1, to just use pinch, set Match Cutoff to 1
