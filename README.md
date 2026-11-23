# DATA 5300: Redhawk Rides

Data preparation and validation for a project examining Redhawk Rides' cancellation fee policy.

The [notebook](./data_prep.ipynb) loads ride requests and experiment assignments, joins them on `rider_id`, checks data quality, and summarizes the experiment groups.

## Run the notebook

1. Install Python dependencies:
   ```bash
   python3 -m pip install jupyter numpy pandas matplotlib scipy
   ```
2. Extract the course-provided `data5300data.zip` into a `data/` folder beside the notebook. It should contain `ride_data.csv` and `experiment_data.csv`.
3. Open `data_prep.ipynb` in Jupyter or VS Code and run all cells from the project directory.

The datasets are excluded from Git because of their size and must be obtained separately.

## Outputs

- [Group summary](./outputs/group_summary.csv): summary statistics by experiment group.
- [Overview plot](./outputs/overview.png): rider counts by group and requests per rider.

Running the notebook regenerates these files.
