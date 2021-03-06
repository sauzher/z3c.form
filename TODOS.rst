======================
To-dos and help wanted
======================

Python 3
--------

- Activate parts as packages get ported.

- Support new schema fields, ``NativeString`` and ``NativeStringLine``.


Framework
---------

- There is only hidden widget templates registered for ``ITextWidget``
  and ``ISelectWidget``. We have to define more hidden widgets.


Widgets
-------

- The MultiWidget should render a minimum number of elements by default
  if the field defines min_length. Also, if user tries to remove elements
  so the number of widgets becomes less than minimum - the widget should
  add widgets to make their number minimum again. (Did you understand
  this?:))

- The MultiWidget should provide a way to reorder elements if used
  for the ISequence field.

- The values defined in "browser" widgets, like ``klass`` or ``onclick``
  should be overridable by value adapters.

- File upload widget and converter should have a "clear current" option
  available to clear current value if there's any and the field is not required.

Documentation
-------------

- Proofread documentation

- Extend API documentation

Samples
-------

Write some samples to show the power of the new widget and form framework.

- Object name as an additional field in an add form


Improvements
------------

Add explicit difference between error and confirmation message e.g.
"There were some errors." and "No changes were applied."

Think about making the framework use NOT_CHANGED on every widget that does not
change it's value.
