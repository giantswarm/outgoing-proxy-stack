# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.17.0] - 2024-07-09

### Changed

- Upgrade `cluster-aws` to use `v25.0.0` GS release

## [0.16.0] - 2024-07-09

### Changed

- Upgrade `cluster-aws` to `0.79.0`

## [0.15.0] - 2024-07-05

### Changed

- Upgrade `cluster-aws` to `0.76.0`

With this version, `cluster-aws` will take over reconciliation of all the default apps.

## [0.14.0] - 2024-07-05

### Changed

This is an intermediate release in the `cluster-aws` [`v0.76.0` upgrade process](https://github.com/giantswarm/cluster-aws/releases/tag/v0.76.0).

:warning: IMPORTANT: :warning: first apply version `0.13.0` of this chart and set `apps.deleteOptions.moveAppsHelmOwnershipToClusterAws` value to `true`, before upgrading to `0.14.0`.

This release will:

- Delete the `default-apps-aws` App CR
- Migrate the cilium app config to the `cluster-aws` configuration

After you've applied this version and the `default-apps-aws` has been removed, upgrade to the next release so `cluster-aws` takes over the default apps.

## [0.13.0] - 2024-07-05

### Changed

In preparation to upgrade `cluster-aws` to [`v0.76.0`](https://github.com/giantswarm/cluster-aws/releases/tag/v0.76.0):

- Upgrade `default-apps-aws` to `0.52.0`
- Upgrade `cluster-aws` to `0.75.0`
- Add `apps.deleteOptions.moveAppsHelmOwnershipToClusterAws` value (defaults to `false`) to be able to migrate default apps to `cluster-aws`. Set this to `true` before upgrading to the next version of this app.

## [0.12.0] - 2024-05-06

### Changed

- Upgrade `squid-proxy` to v0.6.0

## [0.11.4] - 2024-04-09

### Changed

- Upgrade apps

## [0.11.3] - 2024-04-09

### Changed

- Upgrade to 1.25

## [0.11.2] - 2024-04-02

### Changed

- Disable bastion

## [0.11.1] - 2024-04-02

### Changed

- Update cluster to 0.59.1

## [0.11.0] - 2024-02-13

### Changed

- Updated squid proxy to 0.5.4.

## [0.10.1] - 2024-02-09

### Changed

- Updated squid proxy to 0.5.3 with latest allowlist

## [0.10.0] - 2024-02-08

### Changed

- Bump squid version to 0.5.2.

## [0.9.0] - 2024-02-08

### Changed

- Bump squid to 0.5.1.

## [0.8.0] - 2024-02-08

### Changed

- Bump squid to 0.5.0.

## [0.7.0] - 2023-12-07

### Changed

- Change team annotation to phoenix from hydra
- Bump cluster-aws to v0.51.0 and adapt to renamed values
- Bump default-apps-aws to v0.40.0

## [0.6.1] - 2023-07-18

- update squid app to `0.3.4`

## [0.6.0] - 2023-07-13

- changes to upgrade `cluster-aws` version to `0.35.0`

## [0.5.0] - 2023-07-13

- changes to upgrade `cluster-aws` version to `0.34.0`

## [0.4.0] - 2023-07-12

- changes to upgrade `cluster-aws` version to `0.32.0`
- changes to upgrade `default-apps-aws` version to `0.26.0`

## [0.3.0] - 2023-07-12

- changes to upgrade `cluster-aws` version to `0.27.0`

## [0.2.5] - 2023-01-27

- changes to upgrade `cluster-aws` version to `0.22.0`

## [0.2.4] - 2022-12-24

- configure cluster `dnsMode` via values.

## [0.2.3] - 2022-12-24

- propagate `baseDomain` to cluster.

## [0.2.1] - 2022-11-23

- Move `squid-proxy` to `kube-system` namespace and bump version to `0.2.0`.

## [0.2.0] - 2022-11-23

- Set custom cilium api endpoint if the value is non-empty.

## [0.1.13] - 2022-11-23

- Bump versions for components.

## [0.1.11] - 2022-11-23

- Add more custom values.
- Set `baseDomain` for proxy app if the values is not empty.

### Added

- Add aws region and avaiability zones to `values.yaml`.

## [0.1.4] - 2022-09-16

### Changed

- Couple of bugfixes for the proxy settings.

## [0.1.3] - 2022-09-16

## [0.1.2] - 2022-09-16

### Changed

- Rename repository to `outgoing-proxy-stack`.

## [0.1.1] - 2022-09-16

## [0.1.0] - 2022-09-16

- changed: `app.giantswarm.io` label group was changed to `application.giantswarm.io`

[Unreleased]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.17.0...HEAD
[0.17.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.16.0...v0.17.0
[0.16.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.15.0...v0.16.0
[0.15.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.14.0...v0.15.0
[0.14.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.13.0...v0.14.0
[0.13.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.12.0...v0.13.0
[0.12.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.11.4...v0.12.0
[0.11.4]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.11.3...v0.11.4
[0.11.3]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.11.2...v0.11.3
[0.11.2]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.11.1...v0.11.2
[0.11.1]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.11.0...v0.11.1
[0.11.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.10.1...v0.11.0
[0.10.1]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.10.0...v0.10.1
[0.10.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.9.0...v0.10.0
[0.9.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.8.0...v0.9.0
[0.8.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.7.0...v0.8.0
[0.7.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.6.1...v0.7.0
[0.6.1]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.6.0...v0.6.1
[0.6.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.5.0...v0.6.0
[0.5.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.4.0...v0.5.0
[0.4.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.3.0...v0.4.0
[0.3.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.2.5...v0.3.0
[0.2.5]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.2.4...v0.2.5
[0.2.4]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.2.3...v0.2.4
[0.2.3]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.2.2...v0.2.3
[0.2.2]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.2.1...v0.2.2
[0.2.1]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.2.0...v0.2.1
[0.2.0]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.13...v0.2.0
[0.1.13]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.11...v0.1.13
[0.1.11]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.10...v0.1.11
[0.1.10]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.9...v0.1.10
[0.1.9]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.8...v0.1.9
[0.1.8]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.7...v0.1.8
[0.1.7]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.6...v0.1.7
[0.1.6]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.5...v0.1.6
[0.1.5]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.4...v0.1.5
[0.1.4]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.3...v0.1.4
[0.1.3]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.2...v0.1.3
[0.1.2]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.1...v0.1.2
[0.1.1]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/giantswarm/outgoing-proxy-stack/releases/tag/v0.1.0
