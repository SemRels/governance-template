# Setup Checklist

1. Copy `LICENSE`, `.reuse/`, `LICENSES/`, `GOVERNANCE.md`, `SECURITY.md`, `MAINTAINERS.md`, and `CODE_OF_CONDUCT.md` into the target repository.
2. Update `SECURITY.md` so the advisory link points to the target repository.
3. Update `MAINTAINERS.md` with the real maintainers and ownership areas.
4. Review `GOVERNANCE.md` and adjust the overview and scope for the repository type.
5. Update `.reuse/dep5` with the target repository name, contact, source URL, and any extra file patterns.
6. Copy one or more workflow examples from `.github/workflows/template/` into `.github/workflows/` if the target repository should enforce them.
7. If the repository contains nested projects such as `api/`, decide whether they inherit root governance or require a local override file.
8. Commit the changes on `chore/add-governance` and open a PR.
9. Run the repository's existing validation commands.
10. Enable GitHub Security Advisories if they are not already enabled.
