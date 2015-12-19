<img src="https://raw.githubusercontent.com/zorkzou/Molden2AIM/master/m2a-logo.png" />

# Molden2AIM
Molden2AIM is a utility program which can be used to creat AIM-WFN and NBO-47 files from a Molden file.

## Recent Changes
Version 3.2.0 (12/18/2015).

1. Supports the MOLDEN files generated by [NBO6 (> May.2014)](http://nbo6.chem.wisc.edu/).
2. Supports MOLDEN files generated by the [Molden](http://www.cmbi.ru.nl/molden/) program. [Molden](http://www.cmbi.ru.nl/molden/) can read geometry, basis functions, and MOs from the output file of [Gaussian](http://www.gaussian.com/)/[Gamess](http://www.msg.chem.iastate.edu/gamess/)/[Gamess-UK](http://www.cfs.dl.ac.uk/)/[Firefly](http://classic.chem.msu.su/gran/gamess/)/[Q-Chem](http://www.q-chem.com/).
3. The GAB file generated by [Gabedit](http://gabedit.sourceforge.net/) is compatible. Gabedit can read geometry, basis functions, and MOs from the output file of [Gaussian](http://www.gaussian.com/)/[Gamess](http://www.msg.chem.iastate.edu/gamess/)/[Firefly](http://classic.chem.msu.su/gran/gamess/).

Version 3.1.0 (02/25/2015).

1. Supports the MOLDEN files generated by [NWChem](http://www.nwchem-sw.org/), [BDF](http://www.chem.pku.edu.cn/page/ITCC/research/lwj/BDF.htm) (GTO only), [PSI4](http://www.psicode.org/) (spherical functions only), [CADPAC](http://www-theor.ch.cam.ac.uk/software/cadpac.html), and [MRCC](http://www.mrcc.hu/).
2. Bug fix for [NBO6](http://nbo6.chem.wisc.edu/).
3. ReOrdAtm.f90 has been updated for [CFour](http://www.cfour.de/).
4. Check the normalization of [NBO](http://nbo6.chem.wisc.edu/)'s *.47 file.

## Features

1. It converts the data format from Molden to AIM's WFN. The latter format can be read by [AIMPAC](http://www.chemistry.mcmaster.ca/aimpac/imagemap/imagemap.htm), [AIMPAC2](http://www.beaconresearch.org/AIMPAC2/index.html), [AIM2000](http://www.aim2000.de/), [AIMALL](http://aim.tkgristmill.com/), [AIM-UC](http://alfa.facyt.uc.edu.ve/quimicomp/), [DensToolKit](https://sites.google.com/site/jmsolanoalt/software/denstoolkit), [DGrid](http://www.cpfs.mpg.de/~kohout/dgrid.html), [MORPHY98](http://morphy.mib.man.ac.uk/), [Multiwfn](http://multiwfn.codeplex.com/), [PAMoC](http://www.istm.cnr.it/~barz/pamoc/), [ProMolden](http://azufre.quimica.uniovi.es/d-DensEl/), [TopChem](http://www.lct.jussieu.fr/pagesperso/pilme/topchempage.html), [TopMoD](http://www.lct.jussieu.fr/pagesperso/silvi/topmod.html), [Xaim](http://www.quimica.urv.es/XAIM/), and so on. The GAB file of [Gabedit](http://gabedit.sourceforge.net/) is compatible.
2. It saves [NBO](http://nbo6.chem.wisc.edu/)'s *.47 data file. One can do NBO analysis using the stand-alone [GENNBO](http://nbo6.chem.wisc.edu/) program. In addition, the following loop can be performed using [NBO6 (released after May.2014)](http://nbo6.chem.wisc.edu/).

<img src="https://raw.githubusercontent.com/zorkzou/Molden2AIM/master/m2a-loop.png" />

The WFX format will be supported in the future.

## About the Molden file

MOLDEN (or GAB) files generated the the following programs are fully or partly supported by Molden2AIM at present.

* [ACES-II](http://www.qtp.ufl.edu/ACES/) (> 2.9)
* [BDF](http://www.chem.pku.edu.cn/page/ITCC/research/lwj/BDF.htm) (GTO only)
* [CADPAC](http://www-theor.ch.cam.ac.uk/software/cadpac.html)
* [CFour](http://www.cfour.de/)
* [Columbus](http://www.univie.ac.at/columbus/)
* [DALTON](http://daltonprogram.org/) (> 2013)
* [deMon2k](http://www.demon-software.com/public_html/)
* [Firefly](http://classic.chem.msu.su/gran/gamess/), through the utilities [Molden](http://www.cmbi.ru.nl/molden/) or [Gabedit](http://gabedit.sourceforge.net/)
* [Gaussian](http://www.gaussian.com/), through the utilities [Molden](http://www.cmbi.ru.nl/molden/) or [Gabedit](http://gabedit.sourceforge.net/)
* [Gamess](http://www.msg.chem.iastate.edu/gamess/), through the utilities [Molden](http://www.cmbi.ru.nl/molden/) or [Gabedit](http://gabedit.sourceforge.net/)
* [Gamess-UK](http://www.cfs.dl.ac.uk/), through the utility [Molden](http://www.cmbi.ru.nl/molden/)
* [MOLCAS](http://www.teokem.lu.se/molcas/)
* [MOLPRO](http://www.molpro.net/)
* [MRCC](http://www.mrcc.hu/)
* [NBO6](http://nbo6.chem.wisc.edu/) (> May.2014)
* [NWChem](http://www.nwchem-sw.org/), through the [JANPA/nwchem2molden](http://janpa.sourceforge.net/) script
* [ORCA](https://orcaforum.cec.mpg.de/)
* [Priroda](http://wt.knc.ru/wiki/index.php/Priroda_Documentation)
* [PSI4](http://www.psicode.org/)
* [Q-Chem](http://www.q-chem.com/)
* [TeraChem](http://www.petachem.com/)
* [Turbomole](http://www.turbomole.com/)

See readme.html for details.

Examples of applications can be found in W. Zou, D. Nori-Shargh, and J. E. Boggs, On the Covalent Character of Rare Gas Bonding Interactions: A New Kind of Weak Interaction, J. Phys. Chem. A, 2013, 117(1), pp 207-212 at http://pubs.acs.org/doi/abs/10.1021/jp3104535
