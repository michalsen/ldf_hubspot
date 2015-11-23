
Are you running the Hubspot Drupal contrib module and have found this error?

PHP Warning: Unknown: Input variables exceeded 1000. To increase the limit change max_input_vars in php.ini.

**Warning: This module is in early stages of development**

You have too many forms, or form fields!
What are you, crazy???

Well, this may be the fix you need.
It is an addon module to the hubspot drupal contrib that handles each form,
field by field. Add and remove mappings to your hearts content.

Remember when I said earlier that this module was in early dev? Well, I warned you.

First, this uses the existing hubspot module schema (https://www.drupal.org/project/hubspot)
Why does this matter? you'll see if you try and remove a line. That little "x" does nothing right now.
Also, the drupal webform nid column should probably also hold the webform name, for clarity.
Also, you should be allowed to match multiple fields at once. This one at a time process is a P.I.T.A.
Also, and here's the **kicker** but when Submitting, for some reason, an n_ is being prepended to the Hubspot Form GUID, which makes it mostly useless in mapping. I only just noticed this and haven't looked into it yet, but just in case you decide to roll the bones on this module, here's a fair warning: If you still see this message, mostly likely I have not made the changes to the code.

Any questions, hit me up on Twitter (@michalsen)
