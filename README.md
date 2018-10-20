# Bro_Analysis_Scripts

Collection of python scripts I have used to analyse the ouput logs from bro network security monitor (https://www.bro.org/)

1. Create Rate Graphs (create_rate_graphs.py):
  Analyses the rate of ingress and egress packets per second per log file and generates a graph for it.
  It used regex and matplotlib modules to collect the data and create the plots. The plot has the time in seconds on the X-axis and the packets sent at that second on the Y-axis.
  The values for the axes are compressed to 30 second intervals instead of per second to smooth out the graph and reduce the fluctuation. This can be adjusted.
  Changes to be made:
    - Dynamically search for all '.log' files in the folder and create graphs for each file.
    - Add easy options to change the scaling/compression value.
    - Plot each file's output on the same graph with clear labelling and different colours
