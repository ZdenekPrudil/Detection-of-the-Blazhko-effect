# Detection of the Blazhko effect

Simple [Multi-layer Perceptron classifier](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html "MLP sklearn") trained on the *I*-band photometric data from the OGLE-IV survey for the Galactic bulge [[1](https://ui.adsabs.harvard.edu/abs/2019AcA....69..321S/abstract "Cite"),[2](https://ui.adsabs.harvard.edu/abs/2014AcA....64..177S/abstract "Cite")] together with analysis of the Blazhko effect among the fundamental mode RR Lyrae stars [[Prudil et al. (2019).](https://ui.adsabs.harvard.edu/abs/2017MNRAS.466.2602P/abstract "Cite")]. Details on the training and tuning of the hyperparameters can be found here [Prudil & Skarka 2017](https://ui.adsabs.harvard.edu/abs/2019MNRAS.484.4833P/abstract "Cite") in section 2.1.

The code in the enclosed jupyter notebook is compatible with `Python 3.7.3`, `Astropy 4.0.1.` and `Numpy 1.18.5`.

## Usage

The MLP requires six parameters `pulsation period`, `amplitude`, `R21`, `ϕ21`, `R31`, and `ϕ31` derived from *I*-band photometry. The `ϕ21`, and `ϕ31` have to be on the same scale as provided by the OGLE team. These six-parameters are scaled by the enclosed scaler `Blazhko-BLG-StandardScaler.pkl` and then processed by the MLP `MLP-Blazhko-BLG.pkl`. In any case, see the `Classification game.ipynb` for an example on *how-to-...*.

## FYI
If you encounter some problems or have questions, feel free to contact me. Remember, this classifier is trained on fundamental mode RR Lyrae stars in the Galactic bulge, it will not work on the first overtone pulsators. Also, there could be a metallicity component that can change the light curve shape if you use this MLP on RR Lyrae stars with metallicities outside the range of the Galactic bulge RR Lyrae MDF.

If you use this classifier in your work, please cite [Prudil & Skarka 2017](https://ui.adsabs.harvard.edu/abs/2019MNRAS.484.4833P/abstract "Cite") and [Prudil et al. (2019).](https://ui.adsabs.harvard.edu/abs/2017MNRAS.466.2602P/abstract "Cite")
