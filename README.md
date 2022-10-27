# ForwardCharm

This repository served two functions: 
- i) it collects the different predictions charm hadron production at the LHC, and
- ii) it contains a script that plots these predictions (see example below). 

![Example Spectra](https://github.com/KlingFelix/ForwardCharm/blob/main/figures/Example.png)

Currently, we have the following predictions:

**MC Generators: Hadronic Interaction Models**
 - **SIBYLL 2.3d**: *provided by Felix*.
     Dedicated Cosmic Ray MC generator, as implemented in CRMC. For a discussion of charm production, see [arXiv:1806.04140](https://arxiv.org/abs/1806.04140).  
 - **DPMJET 3.2019**: *provided by Felix*.
     Dedicated Cosmic Ray MC generator, as implemented in CRMC. The code and references are available on [GitHub](https://github.com/DPMJET/DPMJET). This generator has not been tuned/validated for charm production.
 - **PYTHIA 8**:  *provided by Felix*.
     Multi purpose MC generator, used to generate Minimum Bias events using the default setting (called the Monash tune). The code and references are available on this  [website](https://pythia.org/manuals/pythia8245/Welcome.html). This generator has not been tuned/validated for charm production.
 - **PYTHIA 8-BLC**: *provided by Felix*.
     Multi purpose MC generator, used to generate Minimum Bias events using a modified modelling of fragmentation (called "String Formation Beyond Leading Colour"). A description of the model can be found in [arXiv:1505.01681](https://arxiv.org/abs/1505.01681). This generator has not been tuned/validated for charm production, but seems to describe the charm hadron flavor ratios better than the Monash tune.
 
 **MC Generators @ LO: Charm Production**
 - **PYTHIA 8**: *provided by Felix*.
     Multi purpose MC generator, used to generate charm events in the hard process  using Monash tune. 
 - **PYTHIA 8-BLC**: *provided by Felix*.
     Multi purpose MC generator, used to generate charm events in the hard process  using "String Formation Beyond Leading Colour" tune.
 - **HERWIG 7**: *provided by Peter*.
     Multi purpose MC generator, used to generate charm events in the hard process  using its default. See [Manual](https://herwig.hepforge.org/) for information. This generator has not been tuned/validated for charm production.
     
 **kT factorization**
 - **kt: ANNA-linear-FF**: *provided by Anna, Atri, Felix and Ina*.
     Prediction based on kT factorization without gluon saturation. Fragmentation modelled using Peterson fragmentation function. 
 - **kt: ANNA-saturation-FF**: *provided by Anna, Atri, Felix and Ina*.
     Prediction based on kT factorization with gluon saturation. Fragmentation modelled using Peterson fragmentation function. 
 - **kt: ANNA-linear-BLC**: *provided by Anna, Atri, Felix and Ina*.
     Prediction based on kT factorization without gluon saturation. Fragmentation modelled using Pythia with the BLC tune. 
 - **kt: ANNA-saturation-BLC**: *provided by Anna, Atri, Felix and Ina*.
     Prediction based on kT factorization with gluon saturation. Fragmentation modelled using Pythia with the BLC tune. 
     
 - **kt: RAFAL-fullkt-MRW**: *provided by Rafal and Antoni*.
     This is the prediction for the standard partonic production mechanism: $g*g* \to c \bar{c}$ obtained within the full kT-factorization approach with the Martin-Ryskin-Watt (MRW) unintegrated gluon (uPDFs). This result is dedicated to the LHCb charm data. See [arXiv: 2210.08890](https://arxiv.org/abs/2210.08890) for details.
 - **kt: RAFAL-hyb-MRW**: *provided by Rafal and Antoni*.
     This is a predcitons for the standard partonic production mechanism: $g*g* \to c \bar{c}$, obtained within the hybrid approach (the small-x gluon is off-shell and the large-x gluon is collinear) with the Martin-Ryskin-Watt (MRW) unintegrated gluons (uPDFs). This result are dedicated to the FPF neutrino flux calculations. See [arXiv: 2210.08890](https://arxiv.org/abs/2210.08890) for details.
 - **kt: KT_RAFAL-hyb-KSlin**: *provided by Rafal and Antoni*.
     Same as above, but with Kutak-Sapeta (KS-linear) unintegrated gluons (uPDFs). See [arXiv: 2210.08890](https://arxiv.org/abs/2210.08890) for details/
 - **kt: RAFAL-hyb+IC-KSlin**: *provided by Rafal and Antoni*.
     This is the prediction that includes intrinsic charm mechanism: $g*c \to g c$, obtained within the hybrid approach with the Kutak-Sapeta (KS-linear) unintegrated gluons (uPDFs) and the for the BHPS[1%] intrinsic charm distribution from the CT14nnloIC PDFs. See [arXiv: 2210.08890](https://arxiv.org/abs/2210.08890) for details.
 - **kt: RAFAL-REC+IC-KSlin**: *provided by Rafal and Antoni*.
    This is the prediction that includes the recombination mechanism: $qg \to Dc$, obtained within the hybrid approach with the Kutak-Sapeta (KS-linear) unintegrated gluons (uPDFs).  See [arXiv: 2210.08890](https://arxiv.org/abs/2210.08890) for details.
     
 **NLO collinear factorization**
 - **nlo: ATRI-FF**: *provided by Anna, Atri, Felix and Ina*.
     NLO prediction obtained by Atri using the CT14 PDF, no kT smearing, $\mu_F=4.5 m_T$ and $\mu_R=1.5 m_T$. Fragmentation modelled using Peterson fragmentation function. 
 - **nlo: ATRI-FF**: *provided by Anna, Atri, Felix and Ina*.
     NLO prediction obtained by Atri using the CT14 PDF, no kT smearing, $\mu_F=4.5 m_T$ and $\mu_R=1.5 m_T$. Fragmentation modelled using Pythia with the BLC tune. 
 - **nlo: YUSEON**: *provided by Yu-Seon, Weidong and Hallsie*.
     NLO prediction obtained by Yu-Seon. Fragmentation modelled using Peterson fragmentation function. 
