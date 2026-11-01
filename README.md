## Lee-Mykland Jump Test (2008)

### Description
A Python-based implementation of the nonparametric, high-frequency jump test introduced in Lee and Mykland (2008). Detects discrete discontinuities and anomalous price movements by standardizing logarithmic returns with an estimate of local/instantaneous volatility and comparing the resulting test statistic against a critical threshold derived from the Gumbel distribution.

Takes a DataFrame as an input and inserts the following columns:
* `log_return`
* `sigma_hat`
* `L`
* `T`
* `J`

The timing, magnitude and direction of detected jumps can therefore be recovered.

### Prerequisites
To execute the code locally, ensure that (1) a Python interpreter is installed on the machine, (2) the Jupyter package and required dependencies (Pandas, NumPy) are installed in the same environment and (3) the Jupyter extension in VS Code is installed.

Install the dependencies using `pip install pandas numpy`

### How to use
To run the code either (i) create a local repository in a dedicated directory on the machine and clone the repo using git clone or (ii) download the repo as a ZIP using the Code button on the top of this page.

After cloning, open the Jupyter Notebook, adjust function parameters and execute the cells.

### Future directions
Future versions could adjust the test for intraday seasonality/periodicity in volatility.

### References
Lee, S. S., & Mykland, P. A. (2008). Jumps in Financial Markets: A New Nonparametric Test and Jump Dynamics. The Review of Financial Studies, 21(6), 2535–2563. https://doi.org/10.1093/rfs/hhm056