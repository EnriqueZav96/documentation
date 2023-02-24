===============
Connect a scale
===============

When using the :abbr:`IoT (Internet of Things)` box in Odoo, there could be the need to use a scale.
Configuring one can be done in a few steps. After setup, the :menuselection:`Point of Sale` app can
be used to weigh products, which is helpful if their prices are calculated based on it.

Connection
==========

To link the scale to the :abbr:`IoT (Internet of Things)` box, connect it with a :abbr:`USB
(Universal Serial Bus)` cable.

.. note::
   In some cases, a serial port to :abbr:`USB (Universal Serial Bus)` adapter may be needed.

If the scale is `compatible with Odoo IoT Box <https://www.odoo.com/page/iot-hardware>`_, there is
no need to set up anything because it will be automatically detected as soon as it is connected.

.. image:: scale/iot-choice.png
   :align: center
   :alt: IOT box auto detection.

The :abbr:`IoT (Internet of Things)` Box may need to be restarted and the scale's drivers may need
to be downloaded to the box in some cases. To do so, go to the :guilabel:`IoT Box Home Page` and
click on :guilabel:`Drivers List`. Then, click on :guilabel:`Load Drivers`.

.. image:: scale/driver-list.png
   :align: center
   :alt: View of the IoT box settings and driver list.

Use a scale in point of sale
============================

To use the scale in the :menuselection:`Point of Sale` app, go to :menuselection:`POS app -->
3-Dot Menu on the POS --> IoT Box section --> Settings/Edit --> enable the IoT Box`
feature. After this is complete the scale device can be set.

.. image:: scale/iot-box-pos.png
   :align: center
   :alt: View of the IoT box feature inside of the PoS settings.

Now, choose the :guilabel:`IoT Box` in the dropdown menu and check the :guilabel:`Electronic Scale`
option. If required, :guilabel:`Save` the changes.

.. image:: scale/electronic-scale-feature.png
   :align: center
   :alt: List of the external tools that can be used with PoS and the IoT box.

The scale is now available in all the :menuselection:`PoS` sessions. Now, if a product has a price
per weight set, clicking on it on the :guilabel:`PoS` screen opens the scale screen, where the
cashier can weigh the product and add the correct price to the cart.

.. image:: scale/scale-view.png
   :align: center
   :alt: Electronic Scale dashboard view when no items are being weighed.
