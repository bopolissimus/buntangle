buntangle
=========

A PHP program that reads a bearerbox.log file, organizes the PDUs and outputs (to stdout) a corresponding log file with PDUs untangled (i.e., fixes nested PDUs, interleaved PDUs, PDUs that have single status lines embedded in them).

We use the third field in the bearerbox log files to associate related lines together.

e.g.,

2013-10-23 08:11:46 [18300] [7] ERROR: connect failed

Initially just a php script that untangles the bearerbox.log file.  We'll be adding other small utilities in the future (e.g., filter out PDU types we don't need).

We'll pull common lines functionality out later if necessary (e.g., is_pdu_start, is_pdu_end).

Initially simple as possible.
