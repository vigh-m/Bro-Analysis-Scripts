# Bro Analysis Scripts

Collection of python scripts I have used to analyse the ouput logs from bro network security monitor (https://www.bro.org/)

** 1. Create Rate Graphs (create_rate_graphs.py): **
  Analyses the rate of ingress and egress packets per second per log file and generates a graph for it.
  It used regex (https://docs.python.org/2/library/re.html) and matplotlib(https://matplotlib.org/) modules to collect the data and create the plots. The plot has the time in seconds on the X-axis and the packets sent at that second on the Y-axis.
  The values for the axes are compressed to 30 second intervals instead of per second to smooth out the graph and reduce the fluctuation. This can be adjusted.
  How To Use:
    - Just download the required script and run it in the folder with the log files.
    - You will have to change the name of the file in the code and edit the graph labels as needed for your file/usecase.
  Changes to be made:
    - Dynamically search for all '.log' files in the folder and create graphs for each file.
    - Add easy options to change the scaling/compression value.
    - Plot each file's output on the same graph with clear labelling and different colours.

## Version
All scripts are in Python 2.7 unless specified otherwise. Tested on Ubuntu 16.04
