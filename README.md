# Memory-Leak-Detector

 MLD - Memory leak detector is a middle man between any C\C++ application and the Kernel\OS.

 In High Level Design - 
* MLD receive Memory Request.
* Forward Memory Request to OS.
* Get the served result of the request.
* Update its ternat data structures to keep track of memory objects used by the application.
* Return Memory Block for Application usage.
