# IPCP-Profetchers

### STEPS EXECUTE THE CODE

- Download [ChampSim repository]( https://github.com/casperIITB/ChampSim)
- Download the source code of IPCP2.0-Pipeline-Predators
- Place `ipcp.l1d_pref`, `ipcp.l2c_pref`, `ipcp.llc_pref` files inside `champsim/ChampSim/prefetcher` folder 
- Download the following traces from this [spec](https://dpc3.compas.cs.stonybrook.edu/champsim-traces/speccpu/), [graph](https://utexas.app.box.com/s/2k54kp8zvrqdfaa8cdhfquvcxwh7yn85/folder/132804598561), [server](https://drive.google.com/file/d/1qs8t8-YWc7lLoYbjbH_d3lf1xdoYBznf/view) and [sat](https://www.dropbox.com/sh/xs2t9y4cuqlgrlp/AACpzGOj6BcSB-BUolGaBjbta?dl=0)
    * `bfs-10.trace.gz`
    * `bfs-14.trace.gz`
    * `602.gcc_s-2226B.champsimtrace.xz`
    * `605.mcf_s-994B.champsimtrace.xz`
    * `620.omnetpp_s-141B.champsimtrace.xz`
    * `kissat-inc-high-30K-1802B.champsimtrace.xz`
    * `client_004.champsimtrace.xz`
    * `server_009.champsimtrace.xz`
- Navigate to the `/champsim/ChampSim` folder, and run:

./build_champsim.sh bimodal no ipcp ipcp ipcp lru 1

- Now, we need to run the `run_champsim.sh` file for the BINARY created in above step and for each TRACE and observe the results:

./run_champsim.sh [BINARY] 30 30 [TRACE] 


### Presentation
 Please refer to this [presentation](https://docs.google.com/presentation/d/17Ht7Z46gF4iBuZEGmhpLKJ5qKuJ02MC2/edit?usp=sharing&ouid=117882488979386791397&rtpof=true&sd=true) and [video](https://drive.google.com/file/d/150QqkiR9GxCrtvydnBwbR-_O4KQnfjAV/view?usp=share_link) for detailed understanding.

### Contributions

| Name                          	| Contribution 	|
|-------------------------------	|--------------	|
| Chanikya (210050053)       	    | Code changes, Presentation, Video |
| Prachothan (210050034)        	| Code changes, Presentation, Video |
| Hemanth (210050117)    	        | Code changes, Presentation, Video |

### References
- [IPCP paper](https://dpc3.compas.cs.stonybrook.edu/pdfs/Bouquet.pdf)
- [IPCP presentation](https://dpc3.compas.cs.stonybrook.edu/slides/bouquet.pdf)
