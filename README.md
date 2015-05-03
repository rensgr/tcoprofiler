# tcoprofiler
simple tco profiling spreadsheet (open document format, ods )


Short explanation on usage of this spreadsheet


"On the density sheet you indicate the virtualization / consolidation capability and capacity of various platforms you are interested in.  It has some simple smartness here and there:  e.g, if a technology allows maximum 10 VM's per cpu and has enough memory to support 100 VM's per cpu, the sheet will never the less use the lowest value, in this case 10 VM's per cpu. The reverse is also true: too little memory to support the # of vm's will result in the lesser number to be used for further calculation

It also supports some other ideas: e.g, you could decide that your automation is so smart that you can turn off unused capacity ( dev / test environments, for example ) : you can specify your estimate of capacity in percents that will be actually used. In that way, you could guestimate wether using expensive tooling to achieve this, could pay for itself by the savings on hard and soft -ware"

"The TCO sheet allows you to specify guestimated costs of hardware, system software, virtualization, system mgmt, middleware and other components like rackspace, network ports. Combining this with the # of  instances you expect, cost of racks, ports and m2 datacenter it calculates a cost number, and the graph shows the breakdown in  software, hardware, system software, data storage and so on...

NB: always check the memory check on row 24 : this might indicate if you are too optimistic about the possibilities......"
The TCO sheet also allows you to see what happens if you have a mix of different technologies, and what happens if you change the percentages of the mix. (e.g, what happens if I run more instances on linux and less on AIX)
input information in the density eval page, then the TCO_v3 page, and you're done
the graphs sheet shows some graphs based on the information in the density eval and TCO_v3 pages

green fields are for inputting data

all others (yellow, orange) contain formula's.
red ones show if your input was valid in some cases


changing stuff: feel free, but let's assume you know what you are doing.....
