Class **Phalcon\\Config**
=========================

*implements* ArrayAccess, Countable

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/config.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Phalcon\\Config is designed to simplify the access to, and the use of, configuration data within applications. It provides a nested object property based user interface for accessing this configuration data within application code.  

.. code-block:: php

    <?php

    $config = new Phalcon\Config(array(
    	"database" => array(
    		"adapter" => "Mysql",
    		"host" => "localhost",
    		"username" => "scott",
    		"password" => "cheetah",
    		"dbname" => "test_db"
    	),
    	"phalcon" => array(
    		"controllersDir" => "../app/controllers/",
    		"modelsDir" => "../app/models/",
    		"viewsDir" => "../app/views/"
    	)
     ));



Methods
-------

public  **__construct** ([*array* $arrayConfig])

Phalcon\\Config constructor



public  **val** (*array* $arrayConfig)

Sets values



public *boolean*  **offsetExists** (*unknown* $property)

Allows to check whether an attribute is defined using the array-syntax 

.. code-block:: php

    <?php

     var_dump(isset($config['database']));




public *mixed*  **get** (*string* $index, [*mixed* $defaultValue])

Gets an attribute from the configuration, if the attribute isn't defined returns null If the value is exactly null or is not defined the default value will be used instead 

.. code-block:: php

    <?php

     echo $config->get('controllersDir', '../app/controllers/');




public *string*  **offsetGet** (*unknown* $property)

Gets an attribute using the array-syntax 

.. code-block:: php

    <?php

     print_r($config['database']);




public  **offsetSet** (*unknown* $property, *mixed* $value)

Sets an attribute using the array-syntax 

.. code-block:: php

    <?php

     $config['database'] = array('type' => 'Sqlite');




public  **offsetUnset** (*unknown* $property)

Unsets an attribute using the array-syntax 

.. code-block:: php

    <?php

     unset($config['database']);




public :doc:`Phalcon\\Config <Phalcon_Config>`  **merge** (:doc:`Phalcon\\Config <Phalcon_Config>` $config)

Merges a configuration into the current one 

.. code-block:: php

    <?php

    $appConfig = new Phalcon\Config(array('database' => array('host' => 'localhost')));
    $globalConfig->merge($config2);




public *array*  **toArray** ()

Converts recursively the object to an array 

.. code-block:: php

    <?php

    print_r($config->toArray());




public  **count** ()

...


public  **__wakeup** ()

...


public static :doc:`Phalcon\\Config <Phalcon_Config>`  **__set_state** ([*array* $properties])

Restores the state of a Phalcon\\Config object



public  **__get** (*unknown* $property)

...


public  **__set** (*unknown* $property, *unknown* $value)

...


public  **__isset** (*unknown* $property)

...


public  **__unset** (*unknown* $property)

...


