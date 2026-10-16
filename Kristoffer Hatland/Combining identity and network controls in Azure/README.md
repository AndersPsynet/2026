# Combining identity and network controls in Azure

**Speaker(s):** Kristoffer Hatland

## Summary

Cloud security in Azure is often approached through either identity or network controls. In practice, both are implemented, but rarely designed together.

This leads to architectures where private endpoints, VNet integration, and managed identities are in place, yet visibility is limited, trust boundaries are unclear, and it becomes difficult to understand how systems actually communicate.

In this session, we will explore how identity and network controls interact in real Azure environments, and how to design architectures that combine both to improve security, visibility, and traceability.

Using concrete Azure scenarios and demos, we will examine how traffic flows through private endpoints and VNet-integrated services, how managed identities govern access, and how these layers can either reinforce or undermine each other depending on design.

We will also walk through common anti-patterns and show how to redesign them to reduce implicit trust and improve observability.

Participants will leave with practical techniques and design patterns for building Azure architectures where identity and network controls work together to create systems that are easier to understand, monitor, and secure.

## Materials

- [Slides (PDF)](slides.pdf)

## Related links

- [Official NIC 2026 agenda](https://nicconf.com/agenda)

## License

These materials are shared under the repository's [MIT license](../../LICENSE). Preserve any required third-party copyright and license notices.
