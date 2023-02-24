====================
Flashing the SD card
====================

In some circumstances, the :abbr:`IoT (Internet of Things)` box's Micro SD Card may need to be
re-flashed to benefit from Odoo's latest :abbr:`IoT (Internet of Things)` image update. This means
that the Odoo :abbr:`IoT (Internet of Things)` box software may need to be updated.

Upgrade from the IoT box homepage
=================================

Go to the :guilabel:`IoT Box Homepage` by navigating to :menuselection:`IoT app --> IoT Boxes` and
clicking on the :guilabel:`IP address` of the :abbr:`IoT (Internet of Things)` box. Then click on
:guilabel:`Update` (next to the version number).

If a new version of the :abbr:`IoT (Internet of Things)` Box image is available, an
:guilabel:`Upgrade to _xx.xx_` button will appear at the bottom of the page. Click this *button* to
upgrade the unit and the :abbr:`IoT (Internet of Things)` box will then flash itself to the new
version of the :abbr:`IoT (Internet of Things)` Box. All of the previous configurations will be
saved.

.. note::
   This process can take more than 30 minutes. Do not turn off or unplug the :abbr:`IoT (Internet of
   Things)` box as it would leave it in an inconsistent state. This means that the :abbr:`IoT
   (Internet of Things)` box will need to be re-flashed with a new image. See
   :ref:`flash_sdcard/etcher`.

.. image:: flash_sdcard/flash-upgrade.png
   :align: center
   :alt: IoT box software upgrade in the IoT box Home Page.

.. _flash_sdcard/etcher:

Upgrade with Etcher Software
============================

.. note::
   A computer is required with a Micro SD card reader/adapter in order to re-flash the Micro SD
   card.

Navigate to Balena's website and download `Etcher <https://www.balena.io/>`_. It's a free and
open-source utility used for burning image files on to drives. Navigate to the :guilabel:`Products`
menu and find `balenaEtcher`. Click the *product* to `download
<https://www.balena.io/etcher#download-etcher>`_. Install and launch the program on the computer.

Then download the version specific :abbr:`IoT (Internet of Things)` image from `nightly
<http://nightly.odoo.com/master/iotbox/>`_.

Image versions on the `nightly <http://nightly.odoo.com/master/iotbox/>`_ website with their
corresponding Odoo database version:

- Odoo V16 --> iotbox-latest.zip
- Odoo V15 --> iotboxv21_10.zip
- Odoo V14 --> iotboxv21_04.zip
- Odoo V13 --> iotboxv20_10.zip

The images should be downloaded and extracted to a convenient file location.

After this step is complete, insert the :abbr:`IoT (Internet of Things)` box's Micro SD card into
the computer or reader. Then open *Etcher* and select :guilabel:`Flash from file`, find and select
the image just downloaded and extracted. Next, select the drive the image should be burned to.
Lastly, click on :guilabel:`Flash` and wait for the process to finish.

.. image:: flash_sdcard/etcher-app.png
   :align: center
   :alt: Balena's Etcher software dashboard.

.. note::
   An alternative software to flashing the Micro SD card with *Balena's Etcher* is *Raspberry
   Pi Imager*. Download the *Raspberry Pi* software `here <https://www.raspberrypi.com/software/>`_.
