# VulnScout SARIF sandbox

Test repository for the VulnScout SARIF export and its upload to GitHub
Code scanning.

- `sbom/host-cluster.rootfs.spdx.json.gz`: SEAPATH v2.0.0 host cluster EFI image
  SBOM (SPDX 3), from https://releases.seapath.org/builds/v2.0.0/
- `assessments/*.openvex.json`: optional custom assessments imported before the
  export, to test how assessed findings show on GitHub.
- `.github/workflows/vulnscout.yml`: scans the SBOM, exports SARIF and uploads it.
