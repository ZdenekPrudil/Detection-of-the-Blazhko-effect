# Detection of the Blazhko effect

Simple [Multi-layer Perceptron classifier](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html "MLP sklearn") trained on the *I*-band photometric data from the OGLE-IV survey for the Galactic bulge [[1](https://ui.adsabs.harvard.edu/abs/2019AcA....69..321S/abstract "Cite"),[2](https://ui.adsabs.harvard.edu/abs/2014AcA....64..177S/abstract "Cite")] together with analysis of the Blazhko effect among fundamental mode RR Lyrae stars [[Prudil et al. (2019).](https://ui.adsabs.harvard.edu/abs/2017MNRAS.466.2602P/abstract "Cite")]. Details on the training and tuning of the hyperparameters can be found here [Prudil & Skarka 2017](https://ui.adsabs.harvard.edu/abs/2019MNRAS.484.4833P/abstract "Cite") in section 2.1.

The code in the enclosed jupyter notebook is compatible with `Python 3.7.3`, `Astropy 4.0.1.` and `Numpy 1.18.5`.

## Usage

The MLP requires six parameters `pulsation period`, `amplitude`, `r`, `\varphi`, `Python 3.7.3`, `Python 3.7.3`, $\theta$, \varphi ,\theta










