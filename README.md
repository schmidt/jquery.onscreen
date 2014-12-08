jQuery.onscreen Plugin
======================

This plugin adds a `:onscreen` pseudo selector to the list of jQuery selectors.
You may use it to test, if an partially visible on the screen.


Examples
--------

Focus the first visible input element:

    $("input:onscreen").first().focus()


Scroll element into view if it was not visible before

    e = $("#calltoaction")

    if (!e.is(":onscreen")) {
        e.get(0).scrollIntoView();
    }


Future work
-----------

* Add tests
* Add `:fullyonscreen` which would match if the whole element is on the screen,
not just parts of it.

Copyright
---------

This code is just a wrapped version of a StackOverflow answer published on
jsfiddle.

Here are the relevant sources:

<dl>
<dt>Author:</dt>
<dd>pebbl http://pebbl.co.uk/</dd>
<dt>StackOverflow:<dt>
<dd>http://stackoverflow.com/q/487073/817202#comment41045330_21627295</dd>
<dt>JSFiddle:<dt>
<dd>http://jsfiddle.net/9nuqpgqa/</dd>
</dl>

