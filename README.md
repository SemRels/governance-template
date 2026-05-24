# SemRels Governance Template

This repository is the canonical template for applying SemRels governance, community health, and REUSE compliance files across organization repositories.

## Included assets

- Apache 2.0 `LICENSE`
- `.reuse/` metadata
- `LICENSES/` license texts
- `GOVERNANCE.md`
- `SECURITY.md`
- `MAINTAINERS.md`
- `CODE_OF_CONDUCT.md`
- `templates/` with governance variants for core, plugin, and simple repositories
- `.github/workflows/template/` with reusable workflow examples
- `SETUP_CHECKLIST.md` for rollout steps

## How to use this template

1. Create a new repository from this template or copy the files into an existing repository.
2. Update repository-specific metadata such as repository URLs, maintainers, and scope statements.
3. Copy a governance variant from `templates/` into `GOVERNANCE.md` if the default file is not the right fit.
4. Enable the workflow templates that fit the target repository.
5. Validate REUSE compliance and open a pull request.

## Repository-specific updates required after copying

- Replace security advisory URLs with the target repository path.
- Update `MAINTAINERS.md` with the actual maintainers for the repository.
- Review `.reuse/dep5` and adjust `Upstream-Name`, contact, and source URL.
- Confirm whether subdirectories such as `api/` inherit root governance or need local override documents.
