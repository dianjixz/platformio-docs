..  Copyright (c) 2014-present PlatformIO <contact@platformio.org>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
       http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

.. _board_atmelavr_sparkfun_megapro8MHz:

SparkFun Mega Pro 3.3V/8MHz
===========================

.. contents::

Hardware
--------

Platform :ref:`platform_atmelavr`: Atmel AVR 8-bit MCUs deliver a unique combination of performance, power efficiency and design flexibility. Optimized to speed time to market-and easily adapt to new ones-they are based on the industry's most code-efficient architecture for C and assembly programming

.. list-table::

  * - **Microcontroller**
    - ATMEGA2560
  * - **Frequency**
    - 8MHz
  * - **Flash**
    - 252KB
  * - **RAM**
    - 8KB
  * - **Vendor**
    - `SparkFun <https://www.sparkfun.com/products/10744?utm_source=platformio.org&utm_medium=docs>`__


Configuration
-------------

Please use ``sparkfun_megapro8MHz`` ID for :ref:`projectconf_env_board` option in :ref:`projectconf`:

.. code-block:: ini

  [env:sparkfun_megapro8MHz]
  platform = atmelavr
  board = sparkfun_megapro8MHz

You can override default SparkFun Mega Pro 3.3V/8MHz settings per build environment using
``board_***`` option, where ``***`` is a JSON object path from
board manifest `sparkfun_megapro8MHz.json <https://github.com/platformio/platform-atmelavr/blob/master/boards/sparkfun_megapro8MHz.json>`_. For example,
``board_build.mcu``, ``board_build.f_cpu``, etc.

.. code-block:: ini

  [env:sparkfun_megapro8MHz]
  platform = atmelavr
  board = sparkfun_megapro8MHz

  ; change microcontroller
  board_build.mcu = atmega2560

  ; change MCU frequency
  board_build.f_cpu = 8000000L

Debugging
---------
:ref:`piodebug` currently does not support SparkFun Mega Pro 3.3V/8MHz board.

Frameworks
----------
.. list-table::
    :header-rows:  1

    * - Name
      - Description

    * - :ref:`framework_arduino`
      - Arduino Wiring-based Framework allows writing cross-platform software to control devices attached to a wide range of Arduino boards to create all kinds of creative coding, interactive objects, spaces or physical experiences.