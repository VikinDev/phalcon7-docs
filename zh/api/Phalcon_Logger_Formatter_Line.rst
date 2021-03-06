Class **Phalcon\\Logger\\Formatter\\Line**
==========================================

*extends* abstract class :doc:`Phalcon\\Logger\\Formatter <Phalcon_Logger_Formatter>`

*implements* :doc:`Phalcon\\Logger\\FormatterInterface <Phalcon_Logger_FormatterInterface>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/logger/formatter/line.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Formats messages using an one-line string


Methods
-------

public  **__construct** ([*string* $format], [*string* $dateFormat])

Phalcon\\Logger\\Formatter\\Line construct



public  **setFormat** (*string* $format)

Set the log format



public *format*  **getFormat** ()

Returns the log format



public  **setDateFormat** (*string* $date)

Sets the internal date format



public *string*  **getDateFormat** ()

Returns the internal date format



public *string*  **format** (*string* $message, *int* $type, *int* $timestamp, *array* $context)

Applies a format to a message before sent it to the internal log



public *string*  **getTypeString** (*integer* $type) inherited from Phalcon\\Logger\\Formatter

Returns the string meaning of a logger constant



protected  **interpolate** (*string* $message, *array* $context) inherited from Phalcon\\Logger\\Formatter

Interpolates context values into the message placeholders



