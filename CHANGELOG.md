# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.14.0] - 2025-07-29

### Changed

- Update to upstream version v0.63.0

## [0.13.4] - 2025-03-17

### Changed

- Add API capabilities check for Kyverno PolicyExceptions before switching to v2.

## [0.13.3] - 2025-03-17

### Changed

- Make `livenessProbe.initialDelaySeconds` configurable.

## [0.13.2] - 2025-02-25

### Changed

- Narrow down CiliumNetworkPolicy egress rule to match DNS service only.
- Narrow down CiliumNetworkPolicy ingress rule to allow traffic from namespace.

## [0.13.1] - 2024-11-05

### Changed

- Use retagged image for `trivy-db`.

## [0.13.0] - 2024-10-23

### Changed

- Update `Trivy` to upstream version v0.56.1.
- Disable PSPs.

## [0.12.0] - 2024-06-06

### Changed

- Remove feature gate from PolicyException and bump it to v2beta1.
- Update `Trivy` to version v0.52.0.

## [0.11.0] - 2024-04-16

### Changed

- Bump `Trivy` to version v0.50.1.

## [0.10.1] - 2024-02-27

### Added

- Add `application.giantswarm.io/team` label to Trivy StatefulSet.

## [0.10.0] - 2024-01-24

### Changed

- Configure `gsoci.azurecr.io` as the default container image registry.
- Bump Trivy to v0.48.3

## [0.9.0] - 2023-10-27

### Changed

- Bump Trivy to v0.45.1

## [0.8.3] - 2023-09-10

### Fixed

- Bring back port 53 in network policies to download database.

## [0.8.2] - 2023-08-22

### Fixed

- Correct DNS port in network policies.

## [0.8.1] - 2023-05-09

### Added

- Add `Cilium Network Policy` to `trivy`.
- Added Kyverno `PolicyException` for `trivy-app`.

### Changed

- Modified the `VerticalPodAutoscaler` to make the Container Policies configurable.
- Moved the `VerticalPodAutoscaler.enabled` flag to `VerticalPodAutoscaler.trivy.enabled` to align with other Apps.

## [0.8.0] - 2023-03-17

### Changed

- Update to upstream version `0.7.0`/app version `0.37.2`.

## [0.7.1] - 2022-11-21

### Changed

- Adds `VerticalPodAutoscaler` to `trivy`

## [0.7.0] - 2022-11-08

### Changed

- Rename Chart name from `trivy-app` to `trivy`.

## [0.6.0] - 2022-09-16

### Changed

- Update to upstream version `0.4.17`/app version `0.30.4`.

## [0.5.0] - 2022-09-09

### Added

- Implement `install-modules` init job to install custom modules on Trivy `0.29.2`.

### Changed

- Update to upstream version `0.4.16`/app version `0.29.2`.

## [0.4.0] - 2022-07-15

### Changed

- Update to upstream version `0.4.13`/app version `0.28.1`.

## [0.3.0] - 2022-04-12

### Changed

- Update to upstream version `0.4.13`/app version `0.25.0`.

## [0.2.0] - 2022-03-23

### Changed

- Build with `app-build-suite` instead of `architect`.
- Update to upstream version `0.4.12`/app version `0.24.0`.

## [0.1.0] - 2021-12-10

### Changed

- Update to upstream version `0.4.8`/app version `0.21.0`.

## [0.0.2] - 2021-11-12

### Changed

- Metadata change: set a specific app icon

## [0.0.1] - 2021-11-01

### Added

- Initial trivy resources.
- Basic NetworkPolicy resources.

[Unreleased]: https://github.com/giantswarm/trivy-app/compare/v0.14.0...HEAD
[0.14.0]: https://github.com/giantswarm/trivy-app/compare/v0.13.4...v0.14.0
[0.13.4]: https://github.com/giantswarm/trivy-app/compare/v0.13.3...v0.13.4
[0.13.3]: https://github.com/giantswarm/trivy-app/compare/v0.13.2...v0.13.3
[0.13.2]: https://github.com/giantswarm/trivy-app/compare/v0.13.1...v0.13.2
[0.13.1]: https://github.com/giantswarm/trivy-app/compare/v0.13.0...v0.13.1
[0.13.0]: https://github.com/giantswarm/trivy-app/compare/v0.12.0...v0.13.0
[0.12.0]: https://github.com/giantswarm/trivy-app/compare/v0.11.0...v0.12.0
[0.11.0]: https://github.com/giantswarm/trivy-app/compare/v0.10.1...v0.11.0
[0.10.1]: https://github.com/giantswarm/trivy-app/compare/v0.10.0...v0.10.1
[0.10.0]: https://github.com/giantswarm/trivy-app/compare/v0.9.0...v0.10.0
[0.9.0]: https://github.com/giantswarm/trivy-app/compare/v0.8.3...v0.9.0
[0.8.3]: https://github.com/giantswarm/trivy-app/compare/v0.8.2...v0.8.3
[0.8.2]: https://github.com/giantswarm/trivy-app/compare/v0.8.2...v0.8.2
[0.8.2]: https://github.com/giantswarm/trivy-app/compare/v0.8.1...v0.8.2
[0.8.1]: https://github.com/giantswarm/trivy-app/compare/v0.8.0...v0.8.1
[0.8.0]: https://github.com/giantswarm/trivy-app/compare/v0.7.1...v0.8.0
[0.7.1]: https://github.com/giantswarm/trivy-app/compare/v0.7.0...v0.7.1
[0.7.0]: https://github.com/giantswarm/trivy-app/compare/v0.6.0...v0.7.0
[0.6.0]: https://github.com/giantswarm/trivy-app/compare/v0.5.0...v0.6.0
[0.5.0]: https://github.com/giantswarm/trivy-app/compare/v0.4.0...v0.5.0
[0.4.0]: https://github.com/giantswarm/trivy-app/compare/v0.3.0...v0.4.0
[0.3.0]: https://github.com/giantswarm/trivy-app/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/giantswarm/trivy-app/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/giantswarm/trivy-app/compare/v0.0.2...v0.1.0
[0.0.2]: https://github.com/giantswarm/trivy-app/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/giantswarm/trivy-app/releases/tag/v0.0.1
