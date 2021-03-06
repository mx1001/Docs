![header](img/banner.gif)

### Booleans

## Hard Ops and Booleans

**Booltool is no longer required** The hotkeys I once used booltool for have been added into the core of hard ops and supports the drawing and interconnecting systems as a result. This allows for deeper interaction and and possible expansions on the workflow independent of changes outside of our control.

The hotkeys are as follows:

- <kbd>ctrl</kbd> + <kbd>numpad minus</kbd> (difference boolean)
- <kbd>ctrl</kbd> + <kbd>numpad plus</kbd> (union boolean)
- <kbd>ctrl</kbd> + <kbd>numpad slash</kbd> (slash boolean)
- <kbd>shift</kbd> + <kbd>alt</kbd> + <kbd>numpad slash</kbd> (inset boolean)

To demonstrate union and difference.

![bool](img/boolean/ll3.gif)

To demonstrate slash.

![bool](img/boolean/ll4.gif)

And inset.

![bool](img/boolean/b6.gif)

As the gif shows you can also use [hopsTool](hopsTool.md) w/ 2 object selection to setup booleans as well.


> Slash is also in the <kbd>Q</kbd> menu when 2 objects are selected.

> <kbd>Hotkeys</kbd> can be quite fast for setting up booleans on the fly.

![bool](img/boolean/ll21.gif)

So while we support booltool and will respect it if enabled, the HOPS boolean system will also set up [drawing](hud.md) and use our [systems](sstatus.md) which extends on what booltool was able to provide.

---

## Using Booleans in Hard Ops

# hotkeys

With 2 or more objects the following hotkeys apply.

- <kbd>ctrl</kbd> + <kbd>numpad minus</kbd> (difference boolean)
- <kbd>ctrl</kbd> + <kbd>numpad plus</kbd> (union boolean)
- <kbd>ctrl</kbd> + <kbd>numpad slash</kbd> (slash boolean)

![bool](img/boolean/ll14.gif)

# <kbd>Q</kbd> menu

With 2 or more objects the <kbd>Q</kbd> menu will show an option for booleans.

![bool](img/boolean/ll5.png)

> I generally use the hotkeys but this is added for additional conveninece.

# <kbd>Shift</kbd> + <kbd>Q</kbd> Pie menu

With 2 or more objects the <kbd>shift</kbd> + <kbd>Q</kbd> menu will show options for booleans.

![bool](img/boolean/ll6.png)

---

## boolshape

When an object is used as a boolean the following things happen:
  - object is converted into a wire
  - object receives the sstatus: boolshape which affects the <kbd>Q</kbd> menu

This means the object has a special <kbd>Q</kbd> menu with options for bevel, solidify and array.
To demonstrate them all at once.

![bool](img/boolean/ll7.gif)

When the logo is red the object is a boolshape. To reset a boolshape just reset the sstatus and convert back into solid in the [settings](settings.md) submenu.

![bool](img/boolean/ll8.gif)


---

# Interactive Boolean

Booleans can typically be used as operations with the post options being adjustable in the F9 panel.

![bool](img/boolean/b1.gif)

Interactive Boolean launches the user into a modal where the operation being performed can be adjusted on the fly.

![bool](img/boolean/b2.gif)

Post adjustment is possible in the F9 panel is available for use in making fine adjustments.

![bool](img/boolean/b3.gif)

---

# Bool Shift

Boolean marked meshes also known as "boolshapes" are capable of transitioning into any other type of cutter.

![bool](img/boolean/b4.gif)

The default shift form is typically slice since the initial goal was classic rebool which was meant to get a slice from a difference at a later time.

![bool](img/boolean/b5.gif)

---

## Material Cutting

With 008 there came the ability to do material cutting. For this you will need materials with viewport colors in order to see visually.

**(<kbd>ctrl</kbd> + <kbd>~</kbd>)** Brings up the [Hard Ops Helper](helper.md)

On the material tab at the bottom is a cut material area.
Requires object to be selected of course.

![bool](img/boolean/ll19.gif)

It is also in the <kbd>N</kbd> panel.

![bool](img/boolean/ll10.gif)

To explain what the options mean:

- All - lists all materials in scene
- Object - lists all material on the object already (never used)

![bool](img/boolean/ll11.png)

- material list - lists materials
- force material button - this is on by default. It forces the material into a new indice for the boolean operation (never disabled)

![bool](img/boolean/ll12.gif)

In the above example I used the <kbd>N</kbd> panel to set up the cutting material.

Material slicing is also supported.

![bool](img/boolean/ll13.gif)

This can come in handy for performing material cuts as a finishing step for detailing and using materials to trim models.

> Notice that I am able to access the helper via the <kbd>ctrl</kbd> + <kbd>~</kbd> , <kbd>N</kbd> panel and mini helper button.

![bool](img/boolean/ll20.gif)

---

# Boolean dots

While hopsTool is active users can select 2 objects and hold <kbd>ctrl</kbd> to bring up boolean dots.
- cut
- join
- slice

are available at this time.

![hotkey](img/hopstool/h8.gif)

Boolshapes also get their own dot which is where the view can get cluttered quickly.

Fade distance can be adjusted if needed and booldots can be turned off if they are getting in the way.

![hotkey](img/hopstool/h9.gif)

---

# Backstory: [Booltool](https://blenderartists.org/forum/showthread.php?336498-BoolTool-0-2&p=2659836&viewfull=1#post2659836)

Before [booltool](https://github.com/vitorbalbio/code/tree/master/BoolTool) existed, adding a boolean to a mesh was similar to the below example.

![bool](img/boolean/ll1.gif)

When [Booltool](https://blenderartists.org/forum/showthread.php?336498-BoolTool-0-2&p=2659836&viewfull=1#post2659836) first came out it caused an explosion of booleans onto the scene. They always existed but there never was an approach to make them so applicable.

> I mention the 0.2 version because it was the last update by original creator vitorbalbio. 0.3 and beyond is now handled by a different person so therefore the tool is different now.

In my personal workflow it introduced the ability use the hotkeys:

- <kbd>ctrl</kbd> + <kbd>numpad minus</kbd> (difference boolean)
- <kbd>ctrl</kbd> + <kbd>numpad plus</kbd> (union boolean)

![bool](img/boolean/ll2.gif)

I used booltool for the longest time in this state without expansion or advancement. I especially used this in conjunction with edge split which made animation a nightmare. However this was the workflow at the time.

It goes without saying booltool had many other features worth checking out but the subtractive behavior was my main focus. I still loved what this tool brought to the table and it also opened my eyes to having mirroring and other tools have the same simplistic behavior.

---
