:tocdepth: 1

.. sectnum::

.. Metadata such as the title, authors, and description are set in metadata.yaml

.. TODO: Delete the note below before merging new content to the main branch.


Abstract
========

To test the functionality of the pneumatic actuators on the M1M3 mirror cell, small perturbations are applied to each of the actuators in turn.  This technote describes those tests and how to access the test results from the EFD.

Introduction
================
The M1M3 mirror cell supports the weight of the M1M3 primary mirror for the Simonyi telescope.  The 17 tons of mirror are supported by 156 pneumatic actuators where 44 are single-axis and provide support only in the axial direction (parallel to the telescope optical axis), 100 are dual-axis providing support in the axial and lateral direction, and 12 are dual-axis providing support in the axial and cross lateral directions.  Figures 1 and 2 show the locations of the actuators.  Figure 2 shows the actuator types.  Note that most of the dual-axis actuators apply force in the +Y direction.  This is because this is the force needed to support the weight of the mirror as the telescope tilts to lower elevations.

.. image:: ./_static/Actuators.png

Figure 1.  A screenshot of the MTM1M3 GUI, showing the actuator locations and IDs.

.. image:: ./_static/Actuator_Types.png

Figure 2. This figure shows the actuator types.


Positioning is provided by 6 hard points in a hexapod configuration which moves the mirror to a fixed operational position that shall be maintained during telescope operations. The remaining optical elements will be moved relative to this position in order to align the telescope optics. Support and optical figure correction is provided by the pneumatic actuators.
Each actuator consists of a piston and valves to apply compressed air on either side of the piston, so that each actuator has the capability to push and pull.
To test the functionality of the actuators, there is a test applied to each actuator which is referred to as a "bump test".  This involves raising the mirror so that the actuators are supporting the mirror, and then applying an additional force of about 200 Newtons in both the positive and negative directions.  For actuators which are dual-axis, the primary actuator (in the axial direction) is bumped first, followed by the secondary actuator.  The bump test can be performed on either a single actuator, or it can be cycled through all of the actuators in succession.


Bump Test Overview
======================

During the bump test, perturbations of about 200 Nt are applied to the actuators for a few seconds.  Figure 3 shows the target forces to be applied, and Figure 4 shows the actual measured forces.

.. image:: ./_static/Bump_Test_Target.png

Figure 3.  This shows the target forces to be applied to the actuators during the bump test of a single actuator.

.. image:: ./_static/Bump_Test_Results.png

Figure 4. This shows the actual measured forces applied by the actuators during the bump test of a single actuator


Bump Test States
=====================

XYZ forces vs Cylinder forces
==============================

Summary
==============

