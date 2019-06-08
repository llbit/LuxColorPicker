# LuxColorPicker

LuxColorPicker is a simple HSV color picker for JavaFX with a highly usable
interface. The main features of LuxColorPicker are:

* Only one color selection mode: Hue/Saturation/Value.
* Minimalistic design: no unnecessary components or text distracting users.
* Large components to improve usability.

LuxColorPicker is available in the Maven Central Repository. Add it to your
project with this dependency:

    se.llbit:luxcp:1.0


If you want to see the color picker in action, there is a demo app in this
repository.  Run the demo app with `./gradlew run`.  Here is a screenshot of
the demo app:

![LuxColorPicker demo](http://llbit.se/wp-content/luxcpdemo.png)


## Why LuxColorPicker?

JavaFX already has a built-in color picker component, so one might wonder why
LuxColorPicker is needed. In my opinion the standard JavaFX color picker is
functional but flawed: I don't like its default color selection mode, and it
has unnecessarily small components which make it fiddly to use.

If you agree with these points, then LuxColorPicker might be the right choice.


## Only HSV

Unlike many other color pickers, LuxColorPicker has only one color selection
mode: Hue/Saturation/Value (HSV). In my opinion the HSV mode is the best
selection mode, making all others useless.


## Large Components

Small interface components are fiddly and less visible than large components.
The smaller a component is, the longer it will take to accurately hit with the
mouse (unless the component touches the edge of the screen). This is not my
opinion, [it's UX science][1].

In LuxColorPicker, all components are oversized compared to most other color
pickers. This not only makes the interface easier to use, but also increases the
visibility of the colors on display. In particular the hue selection bar is
much larger than I have seen in other programs. I made the hue bar this large
because it helps in making the available hues clearly visible.

The preview color swatch is large for the same reason: it is important to
clearly see the current selected color.

![LuxColorPicker UI diagram](http://llbit.se/wp-content/luxcpui.png)


## Usability

There is a "Save" button to confirm the current color selection, but the user
does not need to click it. LuxColorPicker is non-modal and focus-shy: simply
clicking outside the color picker closes it and confirms the selection.
Pressing escape cancels the current selection and closes the color picker. The
buttons are there just for users who have not yet learned the optimal
interactions.


## History and Random Swatches

The only nonessential embellishments in LuxColorPicker are the color swatches
below the preview swatch. These are the history and random swatches. The random
swatches show random colors close to the current selected color, and the
history swatches contain the previously selected colors.

The random colors are useful when you don't know exactly what color you want to
pick - maybe one of the random colors will look nice.


## Change Log

* **1.0.1** The background color of the popup window is now set to the JavaFx
  background color.


[1]: https://www.interaction-design.org/literature/article/fitts-s-law-the-importance-of-size-and-distance-in-ui-design

