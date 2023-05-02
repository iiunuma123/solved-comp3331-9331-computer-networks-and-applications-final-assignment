Download Link: https://assignmentchef.com/product/solved-comp3331-9331-computer-networks-and-applications-final-assignment
<br>
<strong><u>Use separate answer booklet for each section</u></strong>

<span style="font-size: 2.61792em; letter-spacing: -1px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">SECTION 1  – Questions 1 – 4</span>

<span style="font-size: 2em; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">Question 1 (X marks)</span>




An intelligent group of super speedy ants decide to set up a point-to-point link between two ant holes, denoted by hole A and hole B. Suppose the bandwidth of this “link” is 1000bps, or bread crumbs per second (you can imagine that each ant holds a bread crumb, and they leave hole A at a rate of 1000 ants per second). The distance from hole A to hole B is 100 meters, and the ants walk at a speed of 1 m/s.




<ul>

 <li>Calculate the Round Trip Time (RTT) for the link between the two holes.</li>

</ul>




<ul>

 <li>Using the delay as half the RTT (i.e. just going from A to B, not going back), calculate the delay x bandwidth product for the link, in bread crumbs.</li>

</ul>




<ul>

 <li>Suppose the queen ant in hole A sends a messenger ant to Hole B to request 10,000 bread crumbs (remember each ant holds exactly one bread crumb). Assume that 10,000 ants are ready to leave when the messenger arrive. What is the duration of time that will elapse between when the messenger departed the queen (i.e. hole A) and all 10,000 ants have arrived at hole A.</li>

</ul>







<h2>Question 2 (X marks)</h2>




Assume that the SendBase for a TCP Reno sender is currently 4000. The TCP sender has sent four TCP segments with sequence numbers 4000, 4500, 5500 and 7000. The sender then receives a segment with an acknowledgement number 7500 and a receive window 6000. The congestion window, CongWin, is set to 10000 bytes after this ACK is processed. Answer the questions (i)-(iii) assuming that this ACK is processed and no further ACKs are received:




<ul>

 <li>What is the value of SendBase?</li>

 <li>How many bytes in total are sent in the four TCP segments?</li>

 <li>What is the last byte (number) that the TCP sender can send with certainty that the receiver’s buffer will not overflow?</li>

</ul>




Now assume that the sender receives three more TCP segments, such that all three segments have TCP acknowledgement number 7500. Answer the questions (iv)-(v) assuming that all three ACKs are processed and no further ACKs are received:




<ul>

 <li>What is the value of CongWin?</li>

 <li>What is the sequence number of the next segment that will be sent?</li>

</ul>

<strong> </strong>

<strong> </strong>

<h2>Question 3 (X marks)</h2>

<strong> </strong>

In the lecture (and in the text) we observed how the AIMD algorithm implemented by TCP enables two TCP connections sharing a bottleneck link to achieve a fair share of the bottleneck link capacity (see Figure 3.56 in the text). Suppose that instead of a multiplicative decrease TCP decreased the window size by a constant amount. Would the resulting AIAD algorithm converge to an equal share algorithm? Justify your answer using a diagram similar to Figure 3.56.




<strong> </strong>

<h2>Question 4 (X marks)</h2>

<strong> </strong>

Consider that only a single TCP Reno connection uses one 10Mbps link which does not buffer any data. Suppose that this link is the only congested link between the sending and receiving hosts. Assume that the TCP sender has a huge file to send to the receiver and the receiver’s receive buffer is much larger than the congestion window. We also make the following assumptions: each TCP segment is 1,500 bytes; the two-way propagation delay of this connection is 150 msec; and this TCP connection is always in congestion avoidance phase, that is ignore slow start.

<ul>

 <li>What is the maximum window size (in segments) that this TCP connection can achieve?</li>

 <li>What is the average window size (in segments) and average throughput (in bps) of this TCP connection?</li>

 <li>How long would it take for this TCP connection to reach its maximum window again after recovering from a packet loss?</li>

</ul>

PLEASE TURN OVER

<strong><u>Use separate answer booklet for each section</u> </strong>




<h1>SECTION 2  – Questions 5 – 8</h1>

<strong> </strong>

<strong> </strong>

<h2>Question 5 (X marks)</h2>

<strong> </strong>




<ol>

 <li>Consider the network topology shown in the figure above. Show the operation of Dijkstra’s link-state algorithm to compute routes from node A to all destinations.</li>

</ol>




<ol>

 <li>Show the distance table that would be computed by the distance vector algorithm in A once the distance vector algorithm has finished executing. You do not have to run the distance vector algorithm; you should be able to compute the table by inspection. Note: make sure you have a row in the distance table for each neighbour of A.</li>

</ol>




<ol>

 <li>Consider three instances of link failure: (i) Link A-B fails, (ii) Link A-C fails, and (iii) Link A-E fails. In each of these three cases, all links except the one mentioned are still active. In which of the three instances of link failure will the count-to-infinity problem occur? Describe briefly how this problem occurs for the chosen instance. Name a solution to the count-to-infinity problem.</li>

</ol>

<strong> </strong>

<strong> </strong>

<h2>Question 6 (X marks)</h2>




Sheldon Cooper is designing a Network Address Translator (NAT) device to use at home so that multiple computers share a single global IP address (<em>nat ip</em>).




<ul>

 <li>In his first attempt Sheldon designs a NAT, which maps an outgoing {<em>source ip, source port, destination ip, destination port</em>} tuple to {<em>nat ip, new port, destination ip, destination port</em>}. To his surprise, he finds that routers in the Internet drop every packet sent by his NAT.</li>

</ul>

What is missing in Sheldon’s NAT design?

<strong> </strong>

<ul>

 <li>Now assume that Sheldon has corrected the above problem. He now finds that he can successfully browse the Web through the NAT, but he cannot use FTP. Why?</li>

</ul>




<strong> </strong>

<h2>Question 7 (X marks)</h2>




Assume that the forwarding table of a router is as follows:




<table width="302">

 <tbody>

  <tr>

   <td width="161"><strong>Prefix </strong></td>

   <td width="141"><strong>Link Interface </strong></td>

  </tr>

  <tr>

   <td width="161">128.96.170.0/23</td>

   <td width="141">0</td>

  </tr>

  <tr>

   <td width="161">128.96.168.0/23</td>

   <td width="141">1</td>

  </tr>

  <tr>

   <td width="161">128.96.166.0/23</td>

   <td width="141">2</td>

  </tr>

  <tr>

   <td width="161">128.96.164.0/22</td>

   <td width="141">3</td>

  </tr>

  <tr>

   <td width="161">Default</td>

   <td width="141">4</td>

  </tr>

 </tbody>

</table>







Which interface would the datagrams with the following destination IP address be forwarded to?




<ul>

 <li>96.171.92</li>

 <li>96.167.151</li>

 <li>96.163.151</li>

 <li>96.169.192</li>

 <li>96.165.121</li>

</ul>

<strong> </strong>

<strong> </strong>

<h2>Question 8 (X marks)</h2>




Let’s consider the operation of a self-learning Ethernet switch in the context of a network in which 6 nodes labelled A through F are star connected into the self-learning switch (one node connected to each link). Suppose that (i) B sends a frame to E, (ii) E replies with a frame to B, (iii) A sends a frame to B, (iv) B replies with a frame to A. The switch table is initially empty. Show the state of the switch table before and after each of these events. For each of these events, identify the link(s) on which the transmitted frame will be forwarded, and briefly justify your answers.




PLEASE TURN OVER

<strong><u>Use separate answer booklet for each section</u> </strong>




<h1>SECTION 3  – Questions 9 – 12</h1>

<strong> </strong>

<strong> </strong>

<h2>Question 9 (X marks)</h2>




Why doesn’t 802.11 implement collision detection? What compensation mechanism does it implement?




<strong> </strong>

<h2>Question 10 (X marks)</h2>




Consider the wireless network composed of four nodes in Figure 2, which has a linear topology deployed along a highway. The distance between neighbouring nodes is equal. Assume all nodes are using 802.11 MAC with RTS/CTS enabled. The radio range for each node is fixed, and this radio range is slightly longer than the inter-node distance, i.e., each node can reach only its left and right neighbours. Assume that if there are two simultaneous transmissions within the radio range of the receiver, both transmissions will be unsuccessful.













<strong>Figure 2: Figure for Question 10 </strong>




<ul>

 <li>Assume that node A is currently sending a data frame (not an ACK, an RTS, or a CTS) to node B. Node C wants to send a packet to node D. Assume that node C (and only C) ignores the 802.11 MAC and sends the packet. Would C’s packet arrive successfully at D? Would A’s packet arrive successfully at B? Explain your reasoning.</li>

</ul>




<ul>

 <li>Consider the same situation as above except that all nodes are using the 802.11 MAC. Will C start transmission while A is sending the data packet? Why or why not? If not, how does C know that A is transmitting a data frame?</li>

</ul>




<ul>

 <li>Is there any way for C to know when A’s transmission will end? Explain.</li>

</ul>







<h2>Question 11 (X marks)</h2>




Suppose Alice wants to send a message to Bob. Bob has a public-private key pair (K<sup>B</sup><sub>+</sub>, K<sup>B</sup><sub>–</sub>), and Alice has Bob’s certificate. But Alice does not have a public, private key pair. Alice and Bob share the same hash function <em>H(.)</em>

<ul>

 <li>In this situation, is it possible to design a scheme so that Bob can verify that Alice created the message? If so, show how with a block diagram for Alice and Bob.</li>

 <li>Is it possible to design a scheme that provides confidentially for sending the message from Alice to Bob? If so, show how with a block diagram for Alice and Bob.</li>

</ul>


