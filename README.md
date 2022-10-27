# ForwardCharm

This repository served two functions: 
- i) it collects the different predictions charm hadron production at the LHC, and
- ii) it contains a script that plots these predictions (see example below). 

![Example Spectra](https://github.com/KlingFelix/ForwardCharm/blob/main/figures/Example.png)

Currently, we have the following predictions:

**MC Generators: Hadronic Interaction Models**
 - **SIBYLL 2.3d**: *provided by Felix*
     Dedicated Cosmic Ray MC generator, as implemented in CRMC. For a discussion of charm production, see [arXiv:1806.04140](https://arxiv.org/abs/1806.04140).  
 - **DPMJET 3.2019**: *provided by Felix*
     Dedicated Cosmic Ray MC generator, as implemented in CRMC. The code and references are available on [GitHub](https://github.com/DPMJET/DPMJET). This generator has not been tuned/validated for charm production.
 - **PYTHIA 8**:  *provided by Felix*
     Multi purpose MC generator, used to generate Minimum Bias events using the default setting (called the Monash tune). The code and references are available on this  [website](https://pythia.org/manuals/pythia8245/Welcome.html). This generator has not been tuned/validated for charm production.
 - **PYTHIA 8-BLC**: *provided by Felix*
     Multi purpose MC generator, used to generate Minimum Bias events using a modified modelling of fragmentation (called "String Formation Beyond Leading Colour"). A description of the model can be found in [arXiv:1505.01681](https://arxiv.org/abs/1505.01681). This generator has not been tuned/validated for charm production, but seems to describe the charm hadron flavor ratios better than the Monash tune.
 
 **MC Generators @ LO: Charm Production**
 - **PYTHIA 8**: *provided by Felix*
     Multi purpose MC generator, used to generate charm events in the hard process  using Monash tune. 
 - **PYTHIA 8-BLC**: *provided by Felix*
     Multi purpose MC generator, used to generate charm events in the hard process  using "String Formation Beyond Leading Colour" tune.
 - **HERWIG 7**: *provided by Peter*
     Multi purpose MC generator, used to generate charm events in the hard process  using its default. See [Manual](https://herwig.hepforge.org/) for information. This generator has not been tuned/validated for charm production.
