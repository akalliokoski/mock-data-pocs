# SDV PoCs

[The Synthetic Data Vault](https://sdv.dev)

## PoCs
* [Mock diabetes data](https://github.com/akalliokoski/mock-data-pocs/blob/main/sdv-poc/sdv-diabetes-table.ipynb)
  * single table
  * TabularPreset and GaussianCopula models used
* [SDV multi table tutorial](https://github.com/akalliokoski/mock-data-pocs/blob/main/sdv-poc/sdv-multi-table.ipynb)
   * stripped-down version of the HMA1 tutorial

## Notes

### SDV

* Generates synthetic data that mimics the real data
   * Uses modeling techniques to learn the structure and relationships
* Supports tabular, relational and timeseries data
* Learned metadata is manually editable
* Constraints can be used to ensure consistency
* Quality metrics for input and synthetic data by SDMetrics

### SDV Constraints

* Constraints ensure consistency and compliance
* Guide data generation and protect privacy
* SDV supports both built-in and custom constraints
   * Built-in constraints
      * Fixed column combinations
         * e.g. city and country should not be shuffled
      * Inequality comparison
         * e.g. enforce start date < end date
      * Range, fixed increments, ...
   * Custom constraints**

### SDMetrics

* SDMetrics measures quality of input and synthetic data
* Types of metrics:
   * Quality: shape comparison, distributions, parent/child connections
   * Diagnostic: data coverage, min/max ranges, exact matches
   * Privacy: Correct Attribution Probability
   * ...

