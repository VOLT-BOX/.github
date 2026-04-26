# Workflows and automation

Workflow changes in this repository behave like public infrastructure because they can affect organization-wide presentation or shared automation expectations.

## What workflows do here

Typical workflows publish badges, run dependency or security checks, and support org-level automation patterns that other repos may copy.

Even when the automation surface is small, breakage here is highly visible because it can affect the organization profile or any shared GitHub-facing convention derived from this repo.

## Change discipline

Treat workflow edits like production config changes and keep their intent obvious in both file names and documentation.

When editing unfamiliar YAML, validate the workflow path, event triggers, and referenced actions carefully. A minor typo in a public org repo can cause persistent badge failures or broken automation across default branches.

## Scope control

Keep automation in this repo focused on org-level concerns instead of smuggling product-specific deployment logic into the public meta repository.

If a workflow only serves one product repo, it likely belongs there. This repo should hold the pieces that are genuinely shared or publicly relevant.
