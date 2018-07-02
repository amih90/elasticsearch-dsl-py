Elasticsearch DSL Examples
==========================

In this directory you can see several complete examples demonstrating key
concepts and patterns exposed by ``elasticsearch-dsl``.

``alias_migration.py``
----------------------

The alias migration example shows a useful pattern where we use versioned
indices (``test-blog-0``, ``test-blog-1``, ...) to manage schema changes and
hides that behind an alias so that the application doesn't have to be aware of
the versions and just refer to the ``test-blog`` alias for both read and write
operations.

For simplicity we use a timestamp as version in the index name.

``parent_child.py``
-------------------

More complex example highlighting the possible relationships available in
elasticsearch - parent/child and nested.
