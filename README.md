# security-observations

Reusable Crowsi components with independent trust roles. Product registration, CLI composition and installed native helpers belong to [vPremises environment operations](https://github.com/vpremises/environment-operations).

## Packages

- [crowsi-boundary-monitor](crates/crowsi-boundary-monitor): existing crate identity and publication declaration retained.
- [crowsi-host-network-sensor](crates/crowsi-host-network-sensor): existing crate identity and publication declaration retained.
- [crowsi-incident-coordinator](crates/crowsi-incident-coordinator): existing crate identity and publication declaration retained.
- [crowsi-production-assurance](crates/crowsi-production-assurance): existing crate identity and publication declaration retained.

## Verify and explore

```sh
cargo +1.97 test --locked --workspace --all-targets --all-features
cargo +1.97 test --locked --workspace --doc --all-features
```

Each crate README and examples describe its public API. Tests and examples use synthetic state; they do not install an authority, service or maintenance timer. Authority, broker, enforcement, independent verification and recovery retain separate roles. Existing wire/schema identifiers and publish=false declarations are unchanged. Repository relocation does not imply a new registry release. Original public history and license notices are preserved in docs/source-history.
