# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

- configure cluster `dnsMode` via values.

## [0.2.3] - 2022-12-24

- propagate `baseDomain` to cluster.

## [0.2.2] - 2022-11-29

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

[Unreleased]: https://github.com/giantswarm/outgoing-proxy-stack/compare/v0.2.3...HEAD
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
