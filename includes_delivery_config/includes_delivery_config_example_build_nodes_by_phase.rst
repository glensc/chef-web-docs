.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.


The following example shows how to specify build nodes to be used for specific phases.

.. code-block:: javascript

   "build_nodes": {
     "provision": ["name:builder-*-2.delivery.chef.co AND platform_version:14.04"],
     "deploy": ["name:builder-*-2.delivery.chef.co AND platform_version:14.04"],
     "functional": ["name:builder* AND platform_version:14.04 NOT name:builder-*-2.delivery.chef.co"]
   }
