# Contributing to Awesome Post-Server

This catalog highlights software whose **core function does not require a dedicated server**. Decentralized, local-first, self-hosted and peer-to-peer are not synonyms for Post-Server.

## The two-device test

Imagine a desktop and a mobile device, possibly on a local network or behind ordinary firewalls. There is **no third machine**, dedicated NAS, home server, commercial relay, or always-on participant.

Can the participating devices use the application's core feature and retain meaningful data or application state? This is the primary eligibility test. Do not assume internet access, a public rendezvous point, or a separately managed service is always available. Document any connectivity limits honestly; we do not require an impossible guarantee that two disconnected devices can exchange data.

- **Allowed:** A local service bundled with the application on a participant's own device; an ordinary client that also serves its own data; direct P2P; optional, replaceable forwarding by intermittently connected peers; peer-to-peer stores, reconciliation or durable message history.
- **Not allowed:** A separately required authoritative server, relay or account service; a dedicated always-on router/repeater/mailbox; another device that must be provisioned independently; traditional mandatory home-server/client-server architectures, including conventional self-hosted SMTP.
- **Important:** One participating device may be authoritative for its *own* records. The objection is to a mandatory separate service that controls the application for both peers.
- **No automatic inclusion:** A socket chat, VPN, discovery protocol or one-shot stream is not enough simply because it connects peers. The main list is for applications with meaningful enduring state, replicated records, or persistent content—not an unlimited index of trivial connection tools.
- **Still to decide:** Whether an isolated durable file handoff without ongoing replication qualifies. Until decided, classify transfer-only tools as **supporting / review needed** rather than assuming either answer.

Optional infrastructure must be truly optional for the claimed working mode. A relay that is mandatory but operated by a different company is **not** optional. An ordinary client temporarily forwarding for others can be acceptable; a special always-on repeater is not. Distinguish optional bootstrap help from a required rendezvous or name service.

## Catalog boundary: curated applications, not a directory of directories

1. **Main catalog:** Runnable applications whose documented working mode passes the two-device test and has meaningful persistent state. Group by actual user task. A shared protocol is useful context, not evidence of qualification.
2. **External ecosystem indexes:** Link to an established maintained `awesome-*` list for broader protocol, library and accessory coverage. Avoid reproducing its apps, tutorials, bindings, clients, or non-qualifying programs in our site. An external link is **further reading, not endorsement**.
3. **Rare local exceptions:** Consider original comparative work only where it adds substantial unique value absent from an appropriate upstream index. A qualifying application missing upstream belongs directly in our main list, with an upstream suggestion where appropriate; a non-qualifying one belongs upstream or in an issue, **not** in its own published catalog page.

Do **not** create a page merely because a program uses BPv7, IPFS, libp2p, Reticulum or another distributed protocol. Likewise, do not create standalone pages to explain excluded clients, transport libraries, abandoned projects or speculative future modes. Put their architectural assessment in the issue/PR that needs it. Do not add empty categories or extensive navigational scaffolding in advance of eligible entries.

A local ecosystem page is an **exception requiring explicit justification** in the PR: why an existing maintained catalog is insufficient, which genuinely eligible applications it clarifies, and why a brief main-list entry or upstream contribution is not enough.

Independent interoperable implementations in multiple programming languages are **a useful protocol-quality signal, not a hard eligibility rule**. A reusable single-language implementation or a running application can still be important. Bindings around one core do not count as independent implementations when describing language diversity.

## What to record for each proposed entry

Provide evidence in the pull-request description rather than expanding every list item into an essay.

- What can a person actually do today, and what meaningful state persists?
- Which participating device owns authoritative data? Who can replicate it?
- How are peers discovered and connected? Are bootstrap, signalling, Tor nodes, routers, repeaters, storage providers or relays required?
- Can the two-device case function without a third always-on machine? If there are limitations, state them.
- Does the application depend on external sync tooling, a central account, or a fixed server of record?
- Project maturity and **date of assessment** (YYYY-MM-DD), with direct upstream sources and caveats.
- If a technology is merely an accessory, consult or contribute to its upstream ecosystem index instead of adding another page here.

Possible labels are **Qualifies**, **Conditional**, **Supporting** and **Excluded**, independently of maturity (**Alpha**, **Beta**, **Stable**, **Legacy**). A label applies to the **specific mode checked**, not automatically the entire project.

## Existing entries

This policy is a clarification, **not** a blanket assertion that every current entry qualifies. Review current items and open PRs individually before promoting them. In particular, mandatory-relay clients, ordinary self-hosted apps, transfer-only tools, and transport-only systems need fresh scrutiny. Draft PRs that add single-topic reference pages should be converted to a directly qualifying entry, an upstream suggestion, or closed as out of scope.

## Pull requests

Keep changes focused and link direct sources. Include evidence and success criteria in the PR description; record variations or disagreements there. Prefer branches targeting `main` rather than PRs based on other feature branches. Never merge an entry solely because it describes itself as “serverless” or “decentralized.”
