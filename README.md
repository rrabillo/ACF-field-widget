ACF-field-widget
===================


Adds a new field to ACF 5, a widget selector.

----------


Details
-------------

It's all based on the template proposed here, by the ACF's author
[https://github.com/elliotcondon/acf-field-type-template](https://github.com/elliotcondon/acf-field-type-template)

I'm still working on it, but to use it, go to the field declaration, select "Widget" in the "Relationnal" section. Then just choose from wich sidebar you want to get the widgets. 

Then the classical 

    get_field('yourfieldname')
Will output an array containing the infos about the widget. You can now use

    the_widget($className, $instance)
To display it.

the_widget() is an internal wordpress function, so you can use the third arguments.

[https://codex.wordpress.org/Function_Reference/the_widget](https://codex.wordpress.org/Function_Reference/the_widget)