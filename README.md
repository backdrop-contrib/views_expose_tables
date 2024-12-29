Views Expose Tables
===================

This module provides an admin page for architects to choose which tables in a
Backdrop database to expose to Views.

Once seleted, each table has all the fields loaded. The module
detects the data type of the field, and provides appropriate views field, sort,
filter, and argument filters (for example numeric, string, date, or "default").

It also looks for a primary key of the table and if one is found, it sets the
primary key as the base field for a views base table, and makes the table
accessible to views.

If you need more robust data management needs you might try the
Data module. It has a broader focus of data management in general.

Views Expose Tables is focused on simply exposing tables in the Drupal DB to
views. Any table. Its small, efficient, and requires no dependencies (other
than Views). It also doesn't care if the table is "owned" by another module.
Views Expose Tables makes no modifications to the tables or schema.

## Use cases

Some modules store data in tables in the Drupal DB but do not provide Views
exposure. For example, we use the great module https://drupal.org/project/bot.
The bot_log table is not exposed to views but it is convenient to have a view
to filter and sort the log of messages.

### Not recommended

Please note that this module is not recommened. In most cases, it would be best
for the module that provides the database table to also provide the views
integration. Should you discover such a module, it would be best to oepn an
issue in that module's queue instead.

That said, sometimes the messy thing needs to be done. This module is a tool for
that job :)


Requirements <!-- Do not include this section if there are no requirements. -->
------------

This module requires that the following modules are also enabled:

 * Views module


Installation <!-- This section is required. -->
------------

- Install this module using the official Backdrop CMS instructions at
  https://docs.backdropcms.org/documentation/extend-with-modules.

- Visit the configuration page under Administration > Structure > Views >
  Expose Tables (admin/structure/views/expose_tables) and define the tables.

- Any additional steps.


Differences from Drupal 7 <!-- Do not include if there are no differences. -->
-------------------------

- No Ui changes.
- Coding standards cleanup.


Issues <!-- This section is required. -->
------

Bugs and feature requests should be reported in [the Issue Queue](https://github.com/backdrop-contrib/views_expose_tables/issues).


Current Maintainers <!-- This section is required. -->
-------------------

- [Jen Lampton](https://github.com/jenlampton).
<!-- You may also wish to add: -->
- Seeking additional maintainers.


Credits <!-- This section is required. -->
-------

- Ported to Backdrop CMS by [Jen Lampton](https://github.com/jenlampton).
- Maintained for Drupal by [Peter Petrik](https://www.drupal.org/u/slovak).
- Maintained for Drupal by [Mark Hanna](https://www.drupal.org/u/markusa).
- Drupal development sponsored by [Skvare](https://www.drupal.org/skvare).


License <!-- This section is required. -->
-------

This project is GPL v2 software.
See the LICENSE.txt file in this directory for complete text.

<!-- If your project includes other libraries that are licensed in a way that is
compatible with GPL v2, you can list that here too, for example: `Foo library is
licensed under the MIT license.` -->
