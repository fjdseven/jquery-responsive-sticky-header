jQuery responsive sticky header
-----------------------------------------------------------------------------------------

Fixed header with responsive navigation and jQuery to change style at set scroll height.

Installation
------------

After the call to jQuery add the following script:

<pre><code>$(function() {var $document = $(document),
$element = $('#headerContainer'),
  className = 'stickyNav';
$document.scroll(function() {
  if ($document.scrollTop() >= 300) {
$element.addClass("stickyNav" );}
else {
  $element.removeClass("stickyNav");
}});
});
</code></pre>

This will append the class 'stickyNav' to the 'headerContainer' after a scroll of 300 pixels.

As is the CSS will change the navigation bar transparent, but the possibilities are endless.

The responsive navigation will kick in at a viewport width of 694px but this can be changed by amending the Media Query in the CSS file:

<pre><code>@media all and (max-width : 694px) {}
</code></pre>

