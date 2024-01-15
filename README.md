# Memory-Leak-Detector

MLD - Memory leak detector is a middleman between any C\C++ application and the Kernel\OS.

MLD Work includes 3 phases:
* Structure Database - MLD maintains the information about all structures that the application is using.
* Object Database - MLD maintains the information about all objects malloced by the application.
* MLD Algorithm - MLD triggers its algorithm on the Object database to find leaked objects.


In High-Level Design - 
* MLD receives a Memory Request.
* Forward Memory Request to OS.
* Get the served result of the request.
* Update its internal data structures to keep track of memory objects used by the application.
* Return Memory Block for Application usage.
