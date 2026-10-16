# Migrating from Hybrid to Become Fully Entra ID Cloud Native – A Technical Deep Dive

**Speaker(s):** Andy Malone

## Summary

A technical walkthrough of moving from hybrid Active Directory to Microsoft Entra ID cloud-native identity management. Topics include Entra Connect and Cloud Sync, transferring source of authority for groups, users, and contacts, Microsoft Graph, rollback considerations, bulk migration, and planning the retirement of on-premises Active Directory dependencies.

## Materials

- [Slides (PDF)](slides.pdf)

The supplied PDF is titled "Migrating from Hybrid Active Directory to Entra ID Cloud Native. A Technical Deep Dive." This folder and README use the conference program's session title.

## Notes

Only the slides are included; no separate demo scripts are supplied.

The slides contain commands that change identity source of authority, synchronization behavior, and account settings, as well as commands for decommissioning domain controllers. These operations can disrupt authentication and access. Do not run them against production without validating current product guidance, permissions, dependencies, backups, and a tested rollback plan. Use a test environment and least-privilege access when following along.

Some examples use Microsoft Graph beta endpoints. Verify endpoint availability and behavior before use. Relevant Microsoft Entra, Microsoft 365, Intune, or cloud services may require licenses or incur charges.

## Related links

- [Official NIC 2026 agenda](https://nicconf.com/agenda)

## License

These materials are shared under the repository's [MIT license](../../LICENSE). Preserve any required third-party copyright and license notices.
