***

The minimal piece of [[information]] a computer can manipulate is a [[Bit|bit]]. However, in order to be able to do it, computers must address the ***bit's location*** by using a reference point called [[Byte|byte]].

***
*Addresses are represented in hexadecimal notation*
***

[[Memory]] in [[Computer|computers]] consists of an interplay of three actors: [[CPU]], [[RAM]], [[Storage]].
This play follows a ***read-modify-write*** process:

First, *memory* in *secondary storage* is read. Here, *information* is organized in **blocks of bytes**. These blocks can be *randomly accessed*, but their entire contents must be read when trying to modify something within them. 

After reading a block, its contents are placed in a workspace known as *RAM*. Here, each *byte* can be *randomly accessed* and modified.

Finally, the modified block overwrites the previous one in the *secondary storage*. 

The [[CPU]]'s function is to issue the order of reading, and then computing, modifying, and overwriting the data.  

***