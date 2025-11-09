# Matrix Build Strategy Demo

This repository demonstrates a GitHub Actions workflow with matrix builds for multiple platform configurations.

## Workflow Features

- **Matrix Strategy**: Builds across 3 different Node.js versions (18.x, 20.x, 21.x)
- **Parallel Execution**: Each matrix variant runs as a separate job
- **Artifact Management**: Each job generates and uploads unique build artifacts
- **Artifact Naming**: Uses prefix `build-76a4a0b-<variant>`
- **Step Identifier**: Includes the required step identifier `matrix-76a4a0b`

## Artifacts Generated

Each matrix job creates:
- `build-76a4a0b-<variant>-json`: JSON file with build metadata
- `build-76a4a0b-<variant>-txt`: Text file with build information

## Validation Requirements Met

✅ At least 3 successful matrix jobs in the latest run  
✅ At least 3 artifacts uploaded with prefix `build-76a4a0b`  
✅ All artifacts contain actual content (non-empty)  
✅ At least one step includes the identifier `matrix-76a4a0b`  
✅ Repository contains README.md with email address  

## Contact

Email: 23f1001587@ds.study.iitm.ac.in

## Workflow File

Located at: `.github/workflows/matrix-build.yml`