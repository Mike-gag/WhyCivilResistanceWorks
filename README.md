# Why Civil Resistance Works

---

> Gaganis Michail, Pregraduate Student <br />
> Department of Management Science and Technology <br />
> Athens University of Economics and Business <br />
> gaganis.michail@gmail.com

* This respository contains a study on the Civil Resistance movements across the world from 1900-onwards.
* This study takes inspiration from the book [Why Civil Resistance Works](https://www.ericachenoweth.com/research/wcrw) by [Erica Chenoweth](https://www.ericachenoweth.com/) and Maria J. Stephan.
* The research done in this repository is done in the in the context of the *Applied Machine Learning* course, taught by *Mr. Panos Louridas* at the *Department of Management Science and Technology, AUEB*. The assignment can be found [here](/assignment/wcrw_v2.ipynb).
* The study takes place in November-December of `2023`, and references data up until that point in time.

# Data Used 
* For our research we will draw data from the [Nonviolent and Violent Campaigns and Outcomes (NAVCO) Dataset](https://dataverse.harvard.edu/dataverse/navco), and in particular the [NAVCO 1.2 Dataset](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/0UZOTX). In the repository is included the [NAVCO Data dictionary](data/NAVCO_data_dictionary.pdf) that provides more clarity as to what the different variables measure.

* We shall also use data from the [Polity Project](https://www.systemicpeace.org/polityproject.html), available from [Integrated Network for Societal Conflict Research (INSCR)](https://www.systemicpeace.org/inscrdata.html), in particular the [Polity5 Annual Time-Series, 1946-2018](http://www.systemicpeace.org/inscr/p5v2018.xls). The [Polity5 Data Dictionary](data/Polity5DataDictionary.pdf) is provided as well for all intensive purposes.

# To run this notebook
* Dependencies for this notebook are handled by creating a new venv through [Poetry](https://github.com/python-poetry/poetry). To run the notebook with no problems follow the steps below:
0. Install poetry (if you haven't already).
```bash
pip install poetry
```
Verify your installation:
```bash
poetry --version
```
1. Clone the repository locally and move inside the folder:
```bash
git clone https://github.com/Mike-gag/WhyCivilResistanceWorks.git
cd WhyCivilResistanceWorks
```
2. Install all the dependencies needed for the Notebook:
```bash
poetry install
```
3. Activate the venv created by poetry:
```bash
source $(poetry env info -p)/bin/activate
```
4. Run the notebook:
```bash
jupyter lab why_civil_resistance_works/WhyCivilResistanceWorks_gaganis_8200234.ipynb 
``` 
5. (OPTIONAL) If you're encountering problems it may be due to your system using the default Python kernel. In that case, you'll have to add the poetry created kernel to the list of kernels manually:
```bash
python -m ipykernel install --user --name=why-civil-resistance-works-py3.11
``` 
and run the notebook:
```bash
jupyter lab --NotebookApp.kernel_name=why-civil-resistance-works-py3.11 why_civil_resistance_works/WhyCivilResistanceWorks_gaganis_8200234.ipynb
``` 
* The above commands work for linux-based systems (MACos, Ubuntu etc).