# Fictional simulation-deposit example

This example shows how a deposit can be organized. The names and values are invented. It is not necessarily a minimum package.

## Directory tree

```text
example-deposit/
├── README.md
├── LICENSE-data.txt
├── LICENSE-code.txt
├── CITATION.txt
├── software-versions.txt
├── manifest.sha256
├── manuscript-to-files-map.md
├── systems/
│   ├── system-A-start.pdb
│   ├── system-A.top
│   └── nonstandard-parameters/
├── inputs/
│   ├── minimize/
│   ├── equilibrate/
│   └── production/
├── runs/
│   ├── replica-01/
│   ├── replica-02/
│   └── replica-03/
├── analysis/
│   ├── README.md
│   ├── scripts/
│   └── notebooks/
└── results/
    ├── figure-2/
    ├── figure-3/
    └── table-1/
```

## README excerpt

### Scope

This package supports Figures 2 and 3 and Table 1. It contains the system definition, inputs, three independent production replicas, analysis code, and plotted data. Complete trajectories are archived under `runs/`.

### Replicas

| Replica | Starting state | Seed | Production file |
| --- | --- | --- | --- |
| 01 | independently assigned velocities | 10431 | `runs/replica-01/production.xtc` |
| 02 | independently assigned velocities | 20867 | `runs/replica-02/production.xtc` |
| 03 | independently assigned velocities | 31991 | `runs/replica-03/production.xtc` |

The primary analysis pools the three replicas after the equilibration period stated in this README. Replica identifiers remain in the files for provenance and targeted diagnostics.

### Run order

1. Install the software versions listed in `software-versions.txt`.
2. Run the preparation commands listed in `inputs/README.md`.
3. Run each replica with the corresponding production input.
4. Run `analysis/scripts/make_all_results.sh`.
5. Compare generated tables with the files under `results/`.

## Manuscript map excerpt

| Manuscript item | Supporting data | Inputs | Analysis | Output |
| --- | --- | --- | --- | --- |
| Figure 2A | `runs/replica-*/production.xtc` | `inputs/production/` | `analysis/scripts/pool_rmsd.py` | `results/figure-2/pooled-rmsd.csv` |
| Figure 3 | `results/figure-3/pooled-values.csv` | `analysis/README.md` | `analysis/scripts/pool_and_compare.py` | `results/figure-3/panel-data.csv` |
| Table 1 | `results/table-1/pooled-summary.csv` | `analysis/README.md` | `analysis/scripts/table1.py` | `results/table-1/table1.csv` |

## If full trajectories cannot be deposited

The README should state the constraint, identify the omitted files, and provide the claim-supporting analysis data plus a trajectory subset. It should also say where the complete files are retained and how access may be granted.
