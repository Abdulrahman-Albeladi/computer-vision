# computer-vision-reconstructions

<!-- coursework-portfolio-notice:start -->
> [!NOTE]
> **Archived college-work portfolio snapshot.** This repository documents coursework, reconstructed assignments, experiments, and skills developed during university. It is provided for portfolio and educational reference, not as maintained production software. Some projects may require historical dependencies, datasets, SDKs, or manual setup and may not build unchanged on current toolchains.
>
> **Known limitation:** Some reconstructed notebooks may require historical datasets, package versions, or manual path configuration.
<!-- coursework-portfolio-notice:end -->

This repository preserves publish-eligible computer-vision course and research notebook artifacts recovered from CMSC426-related materials. The repository is organized as independent project directories, with original notebook filenames retained for provenance.

The recovered materials are notebook-based. They have not been represented as a unified software package, and no claim is made that they execute unchanged in a current environment.

## Repository layout

```text
projects/
  copy-of-118830360-proj2/
  another-shared-copy-of-shasank-patel-cmsc426-project-1/
  copy-of-shasank-patel-cmsc426-project-2/
  ian-fuller-copy-of-cmsc426-project3/
  copy-of-chris-cmsc426-project4/
docs/
  ownership-and-attribution.md
  notebook-lineage.md
```

See [Project Index](#project-index) for the recovered artifact inventory.

## Setup

The repository does not currently include a pinned Python environment, dependency manifest, dataset bundle, or executable package entry point. Use an isolated environment when inspecting or running notebooks.

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install jupyter
jupyter notebook
```

Open the relevant notebook from its project directory. Install additional dependencies only after reviewing that notebook's imports and setup cells.

Configuration values and local paths should not be committed. If a notebook requires credentials, paths, or dataset locations, provide them through local environment configuration or files excluded by `.gitignore`. `.env.example` is the intended starting point for documenting local configuration without storing secrets.

## Validation status

No successful test run, notebook execution, dependency installation, or dataset reconstruction is documented by the recovered file list. The notebooks should therefore be treated as unvalidated artifacts until they are reviewed and executed in a controlled environment.

Recommended baseline checks are listed in the repository project index and in the machine-readable repository synthesis accompanying this README.

## Data and private-data requirements

The available file inventory does not establish which datasets, image directories, credentials, or external resources are required by each notebook. Some course or research notebooks may refer to local files, shared drives, mounted storage, or data not included in this repository.

Before execution:

1. Review notebook imports, path definitions, and file-loading cells.
2. Identify all missing datasets and external assets.
3. Confirm that any data is authorized for local use and publication.
4. Replace private paths with local configuration where practical.
5. Use synthetic or public substitute data for examples when original data cannot be distributed.

Do not commit private datasets, access tokens, student records, or institution-specific storage paths.

## Limitations

- Project directory names and notebook filenames reflect recovered source names rather than normalized project titles.
- The file list alone does not establish each notebook's assignment topic, algorithmic scope, dependency set, expected outputs, or runtime behavior.
- Original datasets, package versions, runtime environments, and generated outputs may not be present.
- Shared-copy naming may indicate collaboration, duplication, or notebook distribution history; it does not by itself establish authorship or ownership.
- Notebook output cells may contain stale results and should not be interpreted as current validation.

## Provenance and attribution

Original filenames have been retained to preserve lineage. Attribution, ownership review, and notebook-history notes are maintained separately:

- [`docs/ownership-and-attribution.md`](docs/ownership-and-attribution.md)
- [`docs/notebook-lineage.md`](docs/notebook-lineage.md)
- [`LICENSE_REVIEW.md`](LICENSE_REVIEW.md)

The repository intentionally preserves demonstrated work without assigning authorship beyond the available records. Review these documents before redistributing notebooks, code cells, outputs, datasets, or derived work.

## Contributing

Contributions should improve reproducibility without changing historical provenance. In particular:

- Keep recovered notebooks in their original project directories.
- Document dependency and dataset requirements discovered during review.
- Add reproducible scripts or environment files only when supported by the notebook contents.
- Do not add private data, secrets, private filesystem paths, grading materials, or hidden tests.
- Record substantive cleanup or reconstruction decisions in project documentation.

See [`CONTRIBUTING.md`](CONTRIBUTING.md) and [`SECURITY.md`](SECURITY.md) for repository procedures.

## Project index

| Project directory | Recovered notebook | Current status |
| --- | --- | --- |
| `copy-of-118830360-proj2` | `copy-of-118830360-proj2.ipynb` | Preserved notebook artifact; execution not documented. |
| `another-shared-copy-of-shasank-patel-cmsc426-project-1` | `another-shared-copy-of-shasank-patel-cmsc426-project-1.ipynb` | Preserved shared-copy-named notebook artifact; execution not documented. |
| `copy-of-shasank-patel-cmsc426-project-2` | `copy-of-shasank-patel-cmsc426-project-2.ipynb` | Preserved copy-named notebook artifact; execution not documented. |
| `ian-fuller-copy-of-cmsc426-project3` | `ian-fuller-copy-of-cmsc426-project3.ipynb` | Preserved copy-named notebook artifact; execution not documented. |
| `copy-of-chris-cmsc426-project4` | `copy-of-chris-cmsc426-project4.ipynb` | Preserved copy-named notebook artifact; execution not documented. |

For per-project notes, see the project index below.

## Current repository layout

- `docs/` — 2 files
- `projects/` — 5 files

## Public-release status

**PRIVATE ONLY**

Notebook ownership, collaborator permission, and attribution remain unresolved.

This repository uses an all-rights-reserved portfolio license. Review `LICENSE`,
`LICENSE_REVIEW.md`, `THIRD_PARTY_NOTICES.md`, and `OWNERSHIP_REVIEW.md`.
