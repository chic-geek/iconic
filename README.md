# Iconic icons

### What?
Icons in app/sites can be a pain in the butt. Should we use SVG's, PNG's etc? Getting them to line up nicely with text and to be usable in buttons can also be a bit of pain. Most apps/sites require icons, so why not use something that's quick to setup and re-usable. Something like 'Font-Awesome' would be great right? But what about using your own icon font, yea that becomes a bit more hassle, hopefully now not the case be including **Iconic** in your projects.


### Why?
I got a little bored each and every time I setup a new project I'd need to create the same sets of files and styles, and sometimes I'd miss something out and things work as I'd planned. So why not separate this out into a re-usable module.


### How?
* Pretty simple really. `git clone` the directory and slot it into your current sassy project.
* Next `@import "iconic";` into your global stylesheet.
* Open up `_iconic--custom.scss` (this is where you can get configuring), and have a play around with the settings in there.
* Make sure your font is named `#{$fontName}-webfont.#{$ext}`.

When you'd like to use an icon in your markup you can simply use: `<i class="iconic iconic-#{$iconName}"></i>`. Depending on what `iconName` you've used will obviously depend on what Icon gets displayed.

So the
* `.iconic` class makes your element an icon.
* `.iconic-#{$iconName}` then adds the right icon entity to that element.
* `.iconic-lg` will make the icon 3x the size.

That last class also gets added to the `.iconic` element and is a helper class for icon sizing.
A full list of icon sizes are:
* `.iconic-xs` - 75% of the original size.
* `.iconic-sm` - 100% of the original size.
* `.iconic-md` - 2x the size of original icon.
* `.iconic-lg` - 3x the size of original icon.
* `.iconic-xl` - 4x the size of original icon.

**Remember:** You'll need to drop in your own icon names and entity codes into the Sass map before it'll start working but once done, you'll have everything setup ready.

**Notes:** The `test/` directory that's in the root can be removed if not required.

As always... Happy Coding =)
