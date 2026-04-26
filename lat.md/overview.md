# Overview

The `.github` repository is the public organization meta repo for VOLT-BOX and Volt LogIQ branding, profile content, and shared GitHub-facing assets.

## Repository role

This repo owns public org presentation and lightweight shared GitHub content, not runtime code or private operating procedures.

The most visible assets live under `profile/`, where the organization page content and related imagery are maintained. Additional top-level directories such as `aw/` or workflow-support files may exist for automation sources, but the overall character stays public and contributor-facing.

## Public boundary

Anything committed here should be safe for public exposure because the repository is not a private operations space.

Do not treat this repo like a staging area for secrets, one-off runbooks, or internal-only contributor rules. If a change affects member-only processes, it probably belongs in `.github-private` instead.

## Related material

The repository should link outward to private or product-specific documentation when deeper implementation detail is needed.

Use this tree for public messaging, profile polish, and org-visible automation references. Keep internal conventions and sensitive coordination details out of the public repo even when they relate to the same GitHub organization.
