The System for Cross-domain Identity Management (SCIM) specifications provide an HTTP-based protocol (RFC7643) and schema (RFC7644) that makes managing identities in multi-domain scenarios easier.  Since its publication in 2015, SCIM has seen growing adoption.

The first goal of this working group is to incorporate implementation experience; errata and interoperability feedback; and current security and best practices into a revised version of RFC7643 (protocol) and RFC7644 (base schema) suitable for consideration at the Internet Standard level of specification maturity.

Additionally, implementation experience with SCIM has surfaced new use cases and requirements.  The WG will document them in a revision of RFC7642. The WG will also consider publishing extensions to SCIM that have found broad adoption. These extensions may include profiles and schemas for interoperability in additional use cases.

The scope of work for the SCIM WG is:

* Revision of RFC7642 that will:
    * Focus on Use cases and implementation patterns
        * Pull vs. Push based use cases
        * Events and signals use cases
        * Deletion use cases
    * New use cases may be added to the revised RFC
* Revision of RFC7643 and RFC7644 that will include:
    * Profiling SCIM relationships with other identity-centric protocols such as OAuth 2.0, OpenID Connect, Shared Signals, and Fastfed
    * Updates to the evolution of the externalid usage
        * Updates to account state for capturing context of the state or change in state of the users account
* Multi-Value Query Filtering and Paging (will use draft-hunt-scim-mv-paging as input)
* Define a method for coordinating resources between domains:
    * Incremental approach to synchronization
    * Consider building off of RFC8417 and draft-hunt-idevent-scim
* Support for deletion-related goals including:
    * Handling Deletes in SCIM Servers that don’t allow Deletes (Soft Deletes) (will use draft-ansari-scim-soft-delete as input)
* Support for advanced automation scenarios such as:
    * Discovery and negotiation of client credentials
    * Attribute mapping
    * Per-attribute schema negotiation
* Enhance the existing schema to support exchanging of human resources, enterprise group and privileged access management (will use draft-grizzle-scim-pam-ext as input)
