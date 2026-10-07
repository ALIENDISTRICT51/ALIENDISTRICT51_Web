# ALIENDISTRICT51_Web

Static HTML website with shared design tokens and components in `assets/styles.css`.
No package installation, JavaScript bundle, or build step is required. Serve the
repository root with a static HTTP server to preview the root-relative links.

## Project presentation

The homepage adds project cards and an AD51 ecosystem diagram. Detail pages:

- `/projects/nexus/` — workflows, capture, telemetry, and structured data.
- `/projects/brain-vault/` — persistent memory, knowledge, and continuity.
- `/projects/mothership/` — visual Agentic AI OS, NOVA, agents, and runtime.

The existing Agentic Command, privacy, and terms routes remain available. No
relationship between Agentic Command and the three new projects is asserted.

The new descriptions follow the supplied project brief. The repository contains
no implementation documentation for these three projects, so development areas
and future integrations are explicitly described as direction rather than a
verified list of completed features. Check these descriptions against each
project's source documentation when it becomes available.

## Supplied media

All assets are local to `assets/media/`; no external media services are needed.

| Website asset | Supplied source | Placement |
| --- | --- | --- |
| `mothership-interface.png` | Screenshot 2026-10-06 205151.png | Featured homepage card and Mothership detail |
| `nexus-dashboard.png` | Screenshot 2026-08-14 224047.png | Nexus card and detail; CSS trims window chrome |
| `nova-character.png` | 7395919f-b74d-41a1-be34-6eebc970bab4.png | Mothership character direction |
| `nova-character-studies.png` | image-1790295405920.png | Expandable character studies on Mothership detail |
| `brain-vault-poster.jpg` | Frame at 00:10 of Brain_Vault_Project.mp4 | Brain Vault card and video poster |
| `brain-vault-demo.mp4` | Brain_Vault_Project.mp4 | Brain Vault detail video |

The four supplied PNGs are preserved. Cropping uses presentation styles, and
full-size originals can be opened from the detail pages. Character media is
labeled as visual direction rather than a verified production avatar.

The full 1:51 Brain Vault video is encoded as H.264/AAC with a web-compatible
pixel format and fast-start metadata, reducing the original 104 MB file to
approximately 21 MB. It has native controls, inline mobile playback, a poster,
and `preload="none"`; it does not autoplay. A text description accompanies it.
No placeholder media is used.

Project grids stack on small screens, workflow diagrams switch to vertical
steps, and the ecosystem diagram becomes a connected stack. Interaction uses
existing smooth scrolling, restrained hover borders, and a native expandable
character gallery. Existing reduced-motion rules apply to the new styling.

## Validation

Browser validation covered all seven routes at 1440, 768, 390, and 320 px
(28 page/viewport checks), including local links and anchors, image decoding,
horizontal overflow, keyboard-operated mobile navigation, the character gallery,
project navigation, and reduced-motion scrolling. Brain Vault playback and
seeking were checked in a browser. No page, console, or HTTP errors occurred in
the validation server. Desktop and mobile screenshots were visually reviewed.

HTML structure, asset paths, duplicate IDs, and `git diff --check` passed.
There are no configured build, lint, or test commands in this static repository.
