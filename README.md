# TCP-congestion-control-with-reinforcement-learning
Congestion in a computer network occurs when an end system overflows the network with too many packets leading to buffer overflow in the intermediate routers. Due to the finite size of the buffer, the packets are dropped which forces the sender to retransmit. Congestion policy in TCP involves three phases namely, Slow Start, Congestion Avoidance and Congestion Detection. In slow start, initial cWnd is set to 1 and increased exponentially as acknowledgements are received. When the cWnd reaches a threshold, an additive increase policy is adopted referred to as congestion avoidance. In the current TCP congestion control implementation, congestion is assumed to have occurred whenever a packet loss is detected. Congestion detection is carried out by timeouts. When no acknowledgement is received within estimated time, the packet is believed to be lost due to congestion and move to slow start phase which prevents effectively filling the pipe with packets. But not all timeouts are due to congestion (eg. bit errors, handoff, reordering etc.). As networks become more and more complex and dynamic, estimating adaptive congestion window becomes difficult. The features are collected at regular intervals to train the model. The RL based TCP is implemented on top of ns3. The RL based TCP achieves a better throughput and delay compared to TCP NewReno implementation.
