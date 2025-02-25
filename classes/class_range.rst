:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/Range.xml.

.. _class_Range:

Range
=====

**Inherits:** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`EditorSpinSlider<class_EditorSpinSlider>`, :ref:`ProgressBar<class_ProgressBar>`, :ref:`ScrollBar<class_ScrollBar>`, :ref:`Slider<class_Slider>`, :ref:`SpinBox<class_SpinBox>`, :ref:`TextureProgressBar<class_TextureProgressBar>`

Abstract base class for range-based controls.

.. rst-class:: classref-introduction-group

Description
-----------

Range is a base class for :ref:`Control<class_Control>` nodes that change a floating-point :ref:`value<class_Range_property_value>` between a :ref:`min_value<class_Range_property_min_value>` and :ref:`max_value<class_Range_property_max_value>`, using a configured :ref:`step<class_Range_property_step>` and :ref:`page<class_Range_property_page>` size. See e.g. :ref:`ScrollBar<class_ScrollBar>` and :ref:`Slider<class_Slider>` for examples of higher level nodes using Range.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`   | :ref:`allow_greater<class_Range_property_allow_greater>` | ``false``                                                                    |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`   | :ref:`allow_lesser<class_Range_property_allow_lesser>`   | ``false``                                                                    |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`   | :ref:`exp_edit<class_Range_property_exp_edit>`           | ``false``                                                                    |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`max_value<class_Range_property_max_value>`         | ``100.0``                                                                    |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`min_value<class_Range_property_min_value>`         | ``0.0``                                                                      |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`page<class_Range_property_page>`                   | ``0.0``                                                                      |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`ratio<class_Range_property_ratio>`                 |                                                                              |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`   | :ref:`rounded<class_Range_property_rounded>`             | ``false``                                                                    |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`int<class_int>`     | size_flags_vertical                                      | ``0`` (overrides :ref:`Control<class_Control_property_size_flags_vertical>`) |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`step<class_Range_property_step>`                   | ``0.01``                                                                     |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+
   | :ref:`float<class_float>` | :ref:`value<class_Range_property_value>`                 | ``0.0``                                                                      |
   +---------------------------+----------------------------------------------------------+------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +------+--------------------------------------------------------------------------------------------------------------------+
   | void | :ref:`_value_changed<class_Range_method__value_changed>` **(** :ref:`float<class_float>` new_value **)** |virtual| |
   +------+--------------------------------------------------------------------------------------------------------------------+
   | void | :ref:`set_value_no_signal<class_Range_method_set_value_no_signal>` **(** :ref:`float<class_float>` value **)**     |
   +------+--------------------------------------------------------------------------------------------------------------------+
   | void | :ref:`share<class_Range_method_share>` **(** :ref:`Node<class_Node>` with **)**                                    |
   +------+--------------------------------------------------------------------------------------------------------------------+
   | void | :ref:`unshare<class_Range_method_unshare>` **(** **)**                                                             |
   +------+--------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_Range_signal_changed:

.. rst-class:: classref-signal

**changed** **(** **)**

Emitted when :ref:`min_value<class_Range_property_min_value>`, :ref:`max_value<class_Range_property_max_value>`, :ref:`page<class_Range_property_page>`, or :ref:`step<class_Range_property_step>` change.

.. rst-class:: classref-item-separator

----

.. _class_Range_signal_value_changed:

.. rst-class:: classref-signal

**value_changed** **(** :ref:`float<class_float>` value **)**

Emitted when :ref:`value<class_Range_property_value>` changes. When used on a :ref:`Slider<class_Slider>`, this is called continuously while dragging (potentially every frame). If you are performing an expensive operation in a function connected to :ref:`value_changed<class_Range_signal_value_changed>`, consider using a *debouncing* :ref:`Timer<class_Timer>` to call the function less often.

\ **Note:** Unlike signals such as :ref:`LineEdit.text_changed<class_LineEdit_signal_text_changed>`, :ref:`value_changed<class_Range_signal_value_changed>` is also emitted when ``value`` is set directly via code.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_Range_property_allow_greater:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **allow_greater** = ``false``

.. rst-class:: classref-property-setget

- void **set_allow_greater** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_greater_allowed** **(** **)**

If ``true``, :ref:`value<class_Range_property_value>` may be greater than :ref:`max_value<class_Range_property_max_value>`.

.. rst-class:: classref-item-separator

----

.. _class_Range_property_allow_lesser:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **allow_lesser** = ``false``

.. rst-class:: classref-property-setget

- void **set_allow_lesser** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_lesser_allowed** **(** **)**

If ``true``, :ref:`value<class_Range_property_value>` may be less than :ref:`min_value<class_Range_property_min_value>`.

.. rst-class:: classref-item-separator

----

.. _class_Range_property_exp_edit:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **exp_edit** = ``false``

.. rst-class:: classref-property-setget

- void **set_exp_ratio** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_ratio_exp** **(** **)**

If ``true``, and ``min_value`` is greater than 0, ``value`` will be represented exponentially rather than linearly.

.. rst-class:: classref-item-separator

----

.. _class_Range_property_max_value:

.. rst-class:: classref-property

:ref:`float<class_float>` **max_value** = ``100.0``

.. rst-class:: classref-property-setget

- void **set_max** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_max** **(** **)**

Maximum value. Range is clamped if ``value`` is greater than ``max_value``.

.. rst-class:: classref-item-separator

----

.. _class_Range_property_min_value:

.. rst-class:: classref-property

:ref:`float<class_float>` **min_value** = ``0.0``

.. rst-class:: classref-property-setget

- void **set_min** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_min** **(** **)**

Minimum value. Range is clamped if ``value`` is less than ``min_value``.

.. rst-class:: classref-item-separator

----

.. _class_Range_property_page:

.. rst-class:: classref-property

:ref:`float<class_float>` **page** = ``0.0``

.. rst-class:: classref-property-setget

- void **set_page** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_page** **(** **)**

Page size. Used mainly for :ref:`ScrollBar<class_ScrollBar>`. ScrollBar's length is its size multiplied by ``page`` over the difference between ``min_value`` and ``max_value``.

.. rst-class:: classref-item-separator

----

.. _class_Range_property_ratio:

.. rst-class:: classref-property

:ref:`float<class_float>` **ratio**

.. rst-class:: classref-property-setget

- void **set_as_ratio** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_as_ratio** **(** **)**

The value mapped between 0 and 1.

.. rst-class:: classref-item-separator

----

.. _class_Range_property_rounded:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **rounded** = ``false``

.. rst-class:: classref-property-setget

- void **set_use_rounded_values** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_using_rounded_values** **(** **)**

If ``true``, ``value`` will always be rounded to the nearest integer.

.. rst-class:: classref-item-separator

----

.. _class_Range_property_step:

.. rst-class:: classref-property

:ref:`float<class_float>` **step** = ``0.01``

.. rst-class:: classref-property-setget

- void **set_step** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_step** **(** **)**

If greater than 0, ``value`` will always be rounded to a multiple of ``step``. If ``rounded`` is also ``true``, ``value`` will first be rounded to a multiple of ``step`` then rounded to the nearest integer.

.. rst-class:: classref-item-separator

----

.. _class_Range_property_value:

.. rst-class:: classref-property

:ref:`float<class_float>` **value** = ``0.0``

.. rst-class:: classref-property-setget

- void **set_value** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_value** **(** **)**

Range's current value. Changing this property (even via code) will trigger :ref:`value_changed<class_Range_signal_value_changed>` signal. Use :ref:`set_value_no_signal<class_Range_method_set_value_no_signal>` if you want to avoid it.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_Range_method__value_changed:

.. rst-class:: classref-method

void **_value_changed** **(** :ref:`float<class_float>` new_value **)** |virtual|

Called when the **Range**'s value is changed (following the same conditions as :ref:`value_changed<class_Range_signal_value_changed>`).

.. rst-class:: classref-item-separator

----

.. _class_Range_method_set_value_no_signal:

.. rst-class:: classref-method

void **set_value_no_signal** **(** :ref:`float<class_float>` value **)**

Sets the **Range**'s current value to the specified ``value``, without emitting the :ref:`value_changed<class_Range_signal_value_changed>` signal.

.. rst-class:: classref-item-separator

----

.. _class_Range_method_share:

.. rst-class:: classref-method

void **share** **(** :ref:`Node<class_Node>` with **)**

Binds two **Range**\ s together along with any ranges previously grouped with either of them. When any of range's member variables change, it will share the new value with all other ranges in its group.

.. rst-class:: classref-item-separator

----

.. _class_Range_method_unshare:

.. rst-class:: classref-method

void **unshare** **(** **)**

Stops the **Range** from sharing its member variables with any other.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
