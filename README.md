Performance Analysis of TCP Variants & Routing Protocols Using NS2 Simulations              

Aim::
The project is based on implementation of AODV, DSR and DSDV protcols along with tcp agents such as Reno, New Reno, Fack, Sack1 and linux.
The goal of the project is to find the correct combination of routing protocol and TCP variant.


|                Getting Started        |

These steps will help you to run the project on your local machine for testing purposes. The project is tested on Ubuntu 16.04 LTS and MAC operating system.


|                Prerequisites          |

For Ubuntu OS 
>>>  NS 2.35
>>>  GnuPlot build with X-11 or qt5
>>> Perl for running file for additional parameters graph file (optional)

>> For Mac
>>> Latest Xcode
>>> NS 2.35
>>> GNuPlot with Qt
>>> Xquartz
>>> Perl for running file for additional parameters graph file (optional)



|                Installing             |

You need to install all the required pre-requisities and set their environment path respectively. then

1. First of all goto project folder in terminal by CD project command
2. type ns start_program.tcl
3. Provide the input on the screen as required for example 1 for aodv and then 	1 for tcp/reno
4. The resulting files will be generated in folders pdr_files, delay_files, nam_files
5. change directory to pdr_files or delay_files to generate files
6. Type ns rp_graph_generator_delays.tcl for graphs plotting of same Routing protocol with different
	 TCP agents. if error comes then make a folder named "rp" in delay_files and then "graphs" in rp
7. Type ns tcp_graph_generator_delays.tcl for graphs plotting of same TCP protocol with different
	 routing protocols. if error comes then make a folder named "tcp" in delay_files and then "graphs" in tcl folder.
9. change directory to pdr_files
8. Type ns rp_graph_generator_pdr.tcl for graphs plotting of same Routing protocol with different
	TCP agents for calculating pdr. if error comes then make a folder named "rp" in pdr_files and then "graphs" in rp
9. Type ns tcl_graph_generator_pdr.tcl for graphs plotting of same TCP protocol with different
	routing protocols for calculating pdr. if error comes then make a folder named "rp" in pdr_files and then "graphs" in rp




|                Built With             |

Network Simulator 2 - The network simulator used
NAM - Network animator for viewing the simulation animation
GnuPlot - The open source graph plotting framework
TCL - scripting language for network simulation
AWK - Scripting language for manipulating and analyzing data


|                Authors                |

Amarjit Dhillon
Ranjit Singh Saini 



|                Future Work            |

Packet Drop ratio, throughput and other parameters can be calculated for the generated trace file




|		     Acknowledgments            |

We would like to thank people on stackoverflow.com who guided us in solving some intial problems like correct format of trace file and solutions to perl conversion of graph file which can be used for additional parameters like throughput.

Lastly, we would like to thanks our professor to guide us at every step.