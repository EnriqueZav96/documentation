===========================
Use the IoT box for the PoS
===========================

.. image:: pos/pos-connections.png
   :align: center
   :alt: Point of Sale layout diagram.

Prerequisites
=============

Before starting, make sure the following equipment is available:

- An :abbr:`IoT (Internet of Things)` box, with its power adapter
- A computer or tablet with an up-to-date web browser
- An Odoo Online or Odoo instance with the :menuselection:`Point of Sale` and :menuselection:`IoT`
  apps installed or running
- A local network setup with :abbr:`DHCP (Dynamic Host Configuration Protocol)` (this is the default
  setting)
- An RJ45 Ethernet Cable (optional, WiFi is built in)
- Any of the supported hardware (receipt printer, barcode scanner, cash drawer, payment terminal,
  scale, customer display, etc.). The list of supported hardware can be found on the `POS Hardware
  page <https://www.odoo.com/page/point-of-sale-hardware>`_

Setup
=====

To connect hardware to the :abbr:`PoS (Point of Sale)`, the first step is to connect an :abbr:`IoT
(Internet of Things)` box to the database. To do this, follow these instructions: :doc:`Connect an
Internet of Things (IoT) box to the Odoo database <connect>`.

Then, connect the peripheral devices to the :abbr:`IoT (Internet of Things)` box.

-  **Printer**: Connect a supported receipt printer to a :abbr:`USB (Universal Serial Bus)` port or
   to the network and power it on. Refer to
   :doc:`/applications/sales/point_of_sale/restaurant/kitchen_printing`.
-  **Cash drawer**: The cash drawer should be connected to the printer with an RJ25 cable.
-  **Barcode scanner**: Connect the barcode scanner. In order for the barcode scanner to be
   compatible it must end barcodes with an ENTER character (keycode 28). This is most likely the
   default configuration of the barcode scanner.
-  **Scale**: Connect the scale and power it on. Refer to
   :doc:`/applications/productivity/iot/devices/scale`.
-  **Customer Display**: Connect a screen to the :abbr:`IoT (Internet of Things)` box to display the
   :abbr:`PoS (Point of Sale)` order. Refer to :doc:`/applications/productivity/iot/devices/screen`.
-  **Payment terminal**: The connection process depends on the terminal. Refer to the :doc:`payment
   terminals documentation </applications/sales/point_of_sale/payment_methods>`.

Once this is completed, connect the :abbr:`IoT (Internet of Things)` box to the :menuselection:`PoS`
application. To do this, go to :menuselection:`Point of Sale --> Configuration --> PoS`, tick
:guilabel:`IoT Box Devices` and select the devices to be used in this :abbr:`PoS (Point of Sale)`.
:guilabel:`Save` the changes.

.. image:: pos/iot-connected-devices.png
   :align: center
   :alt: Configuring the connected devices in the POS application.

Once set up is done, a new :abbr:`PoS (Point of Sale)` Session can be launched.
