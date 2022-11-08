# File Sync ++

A new Windows 10/11 file sync tool.

#Design Principles

File Sync ++ is designed for a modern Windows, but with the ethos that everything is simple and editable, for example:

* Use of ini files. This allows editing, searching, diffing, merging, copying between machines, and to be easily readable to identify what information is stored for security and privacy.
  
* Security. File Sync ++'s files are stored in a common location (~Documents) and can optionaly be encrypted and compressed. This is an extension to ini files.
  

#Progress

We're still in planning. But Progress so far for 2022...
* [October 31] Core storage engine implemented. Simple to copy, human readable, can handle massive data while staying performant (auto-updating ini files) - yes, ini files !
* [November 7] Enumeration engine implemented and in testing [2 million files]. 
* [Current Task] Testing single threaded enumeration of SSD, HDD, Network NAS, USB Drives, compiler optimizations (for example, itteration vs tail recursion), .Net 6 optimisations. Fault tolerance (i.e. unplug a usb drive), Cancel performance (i.e. large folder enumeration, cancel in the middle), and Progress capability (i.e. seeing what the enumeration is doing at any point without impacting performance or UI).
