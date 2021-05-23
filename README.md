# ScheduleAlgorithms

## First Come First Serve (FCFS)
FCFS is the simplest disk scheduling algorithm. As the name suggests, this algorithm entertains requests in the order they arrive in the disk queue. The algorithm looks very fair and there is no starvation (all requests are serviced sequentially) but generally, it does not provide the fastest service.

###Algorithm:
   Let Request array represents an array storing indexes of tracks that have been requested in ascending order of their time of arrival. ‘head’ is the position of disk head.
   Let us one by one take the tracks in default order and calculate the absolute distance of the track from the head.
   Increment the total seek count with this distance.
   Currently serviced track position now becomes the new head position.
   Go to step 2 until all tracks in request array have not been serviced.
