# NeuroTS

Computational generation of artificial neuronal trees based on the topology of reconstructed cells and their
statistical properties.

## Main usage

Neuronal morphologies provide the foundation for the electrical behavior of neurons, the connectomes they form, and the dynamical properties of the brain. Comprehensive neuron models are essential for defining cell types, discerning their functional roles, and investigating brain disease related dendritic alterations. However, a lack of understanding of the principles underlying neuron morphologies has hindered attempts to computationally synthesize morphologies for decades. We introduce a synthesis algorithm based on a topological descriptor of neurons, which enables the rapid digital reconstruction of entire brain regions from few reference cells. This topology-guided synthesis (NeuroTS) generates dendrites that are statistically similar to biological reconstructions in terms of morpho-electrical and connectivity properties and offers a significant opportunity to investigate the links between neuronal morphology and brain function across different spatio-temporal scales.

NeuroTS can be used for the creation of neuronal morphologies from biological reconstructions. The user needs to extract the distributions of topological and statistical properties using the software in order to create the necessary synthesis inputs. Examples of parameters and distributions can be found in the [Parameters and distributions](https://neurots.readthedocs.io/en/stable/params_and_distrs.html) page of the doc.

Once the `input_parameters` and `input_distributions` have been defined, then NeuroTS can generate one or multiple cells based on the respective inputs. The generated cells can be saved in a variety of file formats (SWC, ASC, H5) so that they can be analyzed and visualized by a variety of different software packages. You can find examples on how to extract distributions, generate cells and run basic validations below.
