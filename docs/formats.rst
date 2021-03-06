Supported File Fomats
=====================


There are several importers (read) and exporters (write) for this object.

* supported file formats for import:

    * .dbc candb / [Vector](http://vector.com)
    * .dbf [Busmaster](https://rbei-etas.github.io/busmaster/) (open source!)
    * .kcd [kayak](http://kayak.2codeornot2code.org/) (open source!)
    * .arxml [autosar](http://autosar.org) system description
    * .yaml dump of the python object
    * .xls(x) excel xls-import, works with .xls-file generated by this lib
    * .sym [peak](http://www.peak-system.com) pcan can description

* supported file formats for export:

 * .dbc
 * .dbf
 * .kcd
 * .xls(x)
 * .json [Canard](https://github.com/ericevenchick/CANard) (open source!)
 * .arxml (very basic implementation)
 * .yaml (dump of the python object)
 * .sym
 * .xml fibex


Export
______

+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|Format|ECUs|Mux  |S/R of Signal|Cycletype|Cycletime|Baudrate |Extended|Byteorder|scaling|min/max|attributes|value tables|signal groups|
+======+====+=====+=============+=========+=========+=========+========+=========+=======+=======+==========+============+=============+
|arxml |    |+    |             |         |         |+        |+       |+        |       |       |          |            |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|dbc   |+   |+    |+            |+        |+        |         |+       |+        |+      |+      |+         |+           |+            |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|dbf   |+   |+    |+            |+        |+        |         |+       |+        |+      |+      |+         |+           |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|json  |    |     |             |         |         |         |        |         |+      |       |          |            |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|kcd   |+   |+    |             |+        |+        |+        |        |         |       |       |          |+           |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|sym   |    |+    |             |         |         |         |+       |+        |+      |+      |          |+           |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|xls(x)|+   |+    |+            |+        |+        |         |        |+        |+      |+      |          |+           |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|csv   |+   |+    |+            |+        |+        |         |        |+        |+      |+      |*         |+           |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|xml   |+   |     |+            |         |         |         |        |+        |+      |+      |          |            |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+



Import
______

+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|Format|ECUs|Mux  |S/R of Signal|Cycletype|Cycletime|Baudrate |Extended|Byteorder|scaling|min/max|attributes|value tables|signal groups|
+======+====+=====+=============+=========+=========+=========+========+=========+=======+=======+==========+============+=============+
|arxml |+   |+    |+            |+        |+        |+        |+       |+        |+      |+      |          |+           |+            |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|dbc   |+   |+    |+            |+        |+        |         |+       |+        |+      |+      |+         |+           |+            |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|dbf   |+   |+    |+            |+        |+        |         |+       |+        |+      |+      |+         |+           |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|kcd   |+   |+    |             |+        |+        |         |        |         |       |       |          |+           |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|sym   |    |+    |             |         |         |         |+       |+        |+      |+      |          |+           |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+
|xls(x)|+   |+    |+            |+        |+        |         |        |+        |p      |p      |          |p           |             |
+------+----+-----+-------------+---------+---------+---------+--------+---------+-------+-------+----------+------------+-------------+

