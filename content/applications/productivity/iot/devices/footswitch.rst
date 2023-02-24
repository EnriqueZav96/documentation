====================
Connect a footswitch
====================

When working in a manufacturing environment, it is always better for an operator to have two hands
available. Odoo's :abbr:`IoT (Internet of Things)` box makes this possible when using a footswitch.

In fact, the operator will be able to go from one screen to another and perform actions by using
their foot and the footswitch. This can be configured in just a few steps in the work center on the
:menuselection:`Manufacturing app`.

Connection
==========

To connect the footswitch to the :abbr:`IoT (Internet of Things)` box, just connect the two by
cable. More often than not this is a :abbr:`USB (Universal Serial Bus)` cable.

If the footswitch is a `supported device <https://www.odoo.com/page/iot-hardware>`_, there is no
need to take further action since it will be automatically detected when connected.

.. image:: footswitch/footswitch-dropdown.png
   :align: center
   :alt: Footswitch recognized on the IoT box.

Link a footswitch to a work center in the manufacturing app
===========================================================

To link the footswitch to an action, it needs to be configured on a work center. Navigate to
:menuselection:`Manufacturing --> Configuration --> Work Centers`. Go to the :guilabel:`Work Center`
the footswitch will be used in and add the device in the :guilabel:`IoT Triggers` tab under
:guilabel:`Device` by selecting :guilabel:`Add a Line`. Then, it can be linked to an
:guilabel:`Action` and optionally a key can be added to trigger it. An example of an
:guilabel:`Action` in the :menuselection:`Manufacturing` app could be the :guilabel:`Validate` or
:guilabel:`Mark as Done` buttons on a manufacturing work order.

.. image:: footswitch/footswitch-example.png
   :align: center
   :alt: Footswitch trigger setup on the Odoo database.

It should be noted that the trigger that is first in the list will be chosen first. So, the order
matters and these triggers can be dragged into order. In the picture above, using the footswitch
will automatically skip the current part of the process currently being worked on.

.. note::
   On the :guilabel:`work order` screen, a status graphic indicates whether the database is
   correctly connected to the footswitch.
