# Smart Beta Portfolio and Portfolio Optimization

### Project Motivation:

1. To build a smart beta portfolio and compare it to a benchmark index.
2. Evaluate the performance of the smart beta portfolio by calculating the tracking error against the index.
3. Build a portfolio using quadratic programming to optimize weights.
4. Rebalance the portfolio and calculate turnover to evaluate performance.
    - Use this metric to find the optimal rebalancing frequency.

### The notebook is separated into two parts:
1. The first part covers data collection and inspection, stock universe construction, benchmark index and initial smart beta ETF weights calculation, cumulative returns calculation on historical window, and tracking error calculation between smart beta ETF and benchmark index.
2. The second part covers rebalancing the ETF to minimize a linear combination of the portfolio variance and the L2 norm between portfolio and benchmark index weights.

### File Descriptions:


    project_3.ipynb
    | - Jupyter notebook containing all data collection, cleaning, and data frame construction, smart beta ETF/portfolio and benchmark index construction, projected returns calculation and comparison, and dynamic portfolio rebalancing and turnover cost calculation.
    helper.py
    |- helper file to abstract some data collection and import statements
    project_helper.py
    |- helper file to abstract graphing functions
    project_test.py
    |- unit tests to flag any major errors
    README.md


### Installations:
- This project requires access to a quotemedia dataset hosted on Udacity instances for the "AI for Trading" course. See [quotemedia api feed](https://www.quotemedia.com/apifeeds) for specifics on quotemedia API access.
- You will need a python environment with the following:
    - see the `requirements.txt` file for specific packages and versions
    - python verson 3.6 or higher

### Instructions:
1. Run each cell in 'project_3.ipynb' in sequence. Make sure the Jupyter notebook is in the same level of the directory as 'helper.py', 'project_helper.py', 'project_tests.py', and 'tests.py'.