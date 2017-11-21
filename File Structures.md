# Directory Structure



```assembly
project/
|-- core/
|	|-- agile/
|	|-- easypost/
|	|-- mailchimp/
|	|-- mailgun/
|	|-- unleashed/
|	|--  ...
|
|-- library/
|	|-- css/
|	|-- fonts/
|	|-- images/
|	|-- js/
|	|-- sass/
|	|--  ...
|
|	vendor/
|	woocommerce/
|	style.css
|	screenshot.png
|	404.php
|	footer.php
|	functions.php
|	...
```



### /Core

The core folder will include all custom backend php scripts we write that gets called into `functions.php`. This applies to all the functions that were tpreviously in /library (including the /inc sub directory), and the plugin specific scripts in the root folder. Only exceptions to this will be functions which are required to be in functions.php in order to work.

This directory will be further divided to better organise the scripts. A file autoloader script can then be used to include all files without having to manually include each one into functions.php. Files which start with an underscore will be ignored from the the include process.



### /Library

Library will continue to host all front-end elements of the site.



/Vendor

All plugins loaded by composer

/woocommerce

Woocommerce template overrides