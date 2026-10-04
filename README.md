# CodeML 2026
## Jadco challenge - Collection Équinoxe
Our task was to:
- estimate Collection Équinoxe’s 2026 rent increase using the history of six buildings in Québec and Ontario
- define the increase measured and justify method

To use the notebook, you must be added as one of the owners of GCP project. Feel free to reach out and we
will be happy to add you.

The libraries used are mostly the ones provided through Google Colab Entreprise. However, you do need to
install the tabpfn-client for our regression model. This also requires a (free!) api key, which we are also
happy to provide.

Other than the 4 datasets that Jadco provided us with, we also sourced floor plans from Jadco's website to
group individual units together, and we used data from StatCan and CMHC for macroeconomic indices. Our full
list of datasets can be found through https://console.cloud.google.com/storage/browser/codeml26 (must also
be authenticated).

Special thanks to Claude Code for generating the charts found in our notebook.
