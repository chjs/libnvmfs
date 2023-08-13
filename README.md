# Libnvmfs
Fast non-volatile memory (NVM) technology changes the landscape of file systems.
A series of research efforts to overcome the traditional file system designs that limit NVM performance.
This research has proposed NVM-optimized file systems to leverage the favorable features of byte-addressability, low-latency, and high scalability.
The work tailors the file system stack to reduce the software overhead in using fast NVM.
As a further step, NVM IO systems use the memory-mapped interface to fully capture the performance of NVM.
However, the memory-mapped interface makes it difficult to manage the consistency semantics of NVM, as application developers need to consider the low-level details.
In this work, we propose Libnvmfs, an extended user-level memory-mapped IO, which provides failure-atomicity and frees developers from the crash-consistency headaches.
Libnvmfs reconstructs a common data IO path with memory-mapped IO, providing better performance and scalability than the state-of-the-art NVM file systems.
