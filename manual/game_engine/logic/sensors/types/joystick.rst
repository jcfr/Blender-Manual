
***************
Joystick Sensor
***************

.. figure:: /images/bge_sensor_joystick1.jpg
   :width: 200px

   Joystick sensor.


The *Joystick* sensor triggers whenever the joystick moves.
It also detects events on a range of ancillary controls on the joystick device (hat, buttons,
etc.). More than one joystick may be used (see "Index").
The exact layout of the joystick controls will depend on the make and model of joystick used.

See :doc:`Sensor Common Options </game_engine/logic/sensors/common_options>` for common options.

Special Options:

Index
   Specifies which joystick to use.
All Events
   Sensor triggers for all events on this joystick's current type.


.. figure:: /images/bge_sensor_joystick_event.jpg
   :width: 200px

   Joystick Events.


Event Type
   A menu to select which joystick event to use.


.. rubric:: Single Axis

.. figure:: /images/bge_sensor_joystick_singaxis.png
   :width: 200px

   Joystick Single Axis.


Single Axis
   Detect movement in a single joystick Axis.

   Axis Number
      - 1 = Horizontal axis (left/right)
      - 2 = Vertical axis (forward/back)
      - 3 = Paddle axis up/down
      - 4 = Joystick axis twist left/right
   Axis Threshold
      Threshold at which joystick fires (Range 0 - 32768)


.. rubric:: Hat

.. figure:: /images/bge_sensor_joystick_hat.png
   :width: 200px

   Joystick Hat.


Hat
   Detect movement of a specific hat control on the joystick.

   Hat number
      Specifies which hat to use (max. 2).
   Hat Direction
      Specifies the direction to use: up, down, left, right, up/right, up/left, down/right, down/left.


.. rubric:: Axis

.. figure:: /images/bge_sensor_joystick_axis.jpg
   :width: 200px

   Joystick Axis.


Axis
   Axis Number
      Specifies the axis (1 or 2).
   Axis Threshold
      Threshold at which joystick fires (Range 0 - 32768).
   Axis Direction
      Specifies the direction to use:

      - (Axis Number = 1) Joystick Left, Right, Up, Down
      - (Axis Number = 2) Paddle upper (Left); paddle Lower (Right);
      - Joystick twist left (Up) Joystick twist right (Down)


.. rubric:: Button

.. figure:: /images/bge_sensor_joystick1.jpg
   :width: 200px

   Joystick Button.


Button
   Specify the *button number* to use.
