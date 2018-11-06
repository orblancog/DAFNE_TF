DAFNE_TF
=======

The main file is job.madx.
DAFNE has two main ring MRe and MRp. Here is the model of the MRp (positron ring).
Linear optics should be OK, but multipoles might not because they come from my
own translator from mad -> madx.

Files :
* cur.madx : contains the quadrupoles and correctors strength. K1 is proportional to these magnet currents.
* bendx_siddarta1 : some dipoles model
* wig   : wiggler model
* kick  : injection kickers
* bpm   : bpms and rf cavity
* drift : drifts
* chv   : horizontal and vertical correctors
* sxp   : sextupoles
* skew  : skew quadrupoles
* quad  : quads during the siddharta experiment
* ir1   : ir1_region configuration, where experiments are installed
* ir2   : ir2_region. Not used. Beams are separated.
* ring  : the line declaration
* p_loc : parameters
* aper  : contains the MRp apertures

The lattice starts at the injection point. IP1 is at about 25m downstream.

This model includes the apertures of QF1, QD0, wigglers and some of the BPMs. However, the beam pipe can be approximated to constant 4cm radius, except in the wigglers where it is reduced to about 2cm, and also the IP1 where it is reduced and assymetrically placed.
A good diagram can be seen if Fig. 14 of the publication Boscolo, Manuela. (2012). Monte Carlo simulation for the Touschek effect with the crab-waist scheme. Physical Review Special Topics - Accelerators and Beams. 15. 10.1103/PhysRevSTAB.15.104201.

oblancog 2018/OCT/16 First Release

oblancog 2018/NOV/02 Adding BPM apertures and limits on gradients
