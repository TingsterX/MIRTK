:orphan:

.. Auto-generated by help-rst from "mirtk compose-maps -h" output

compose-maps
============

.. program:: compose-maps


Synopsis
--------

::

    compose-maps <f1> <f2>... <g>


Description
-----------

.. include:: _descriptions/compose-maps.rst



Standard options
----------------

.. option:: -v, -verbose [n]

   Increase/Set verbosity of output messages. (default: 0)

.. option:: -debug [level]

   Increase/Set debug level for output of intermediate results. (default: 0)

.. option:: -version [major.minor]

   Print version and exit or set version to emulate.

.. option:: -revision

   Print revision (or version) number only and exit.

.. option:: -h, -help

   Print help and exit.


Examples
--------


Example 1
~~~~~~~~~

**Command**::

      compose-maps surface-to-disk.vtp 'InverseStereographicProjection(pole=N,r=1)' surface-to-southern-hemisphere.vtp

**Output/Description**::

    
          Composes the given input surface map which maps each point on a surface embedded in 3D
          Euclidean space to the unit disk with an inverse stereographic projection from the north pole
          to the plane containing the disk. The resulting piecewise linear surface map projects the
          points onto the southern hemisphere of the unit sphere. The default radius, 'r', is equal
          to the maximum distance of the points from the origin along the x and y axis, respectively.
