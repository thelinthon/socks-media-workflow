# Maintenance and Capability Self-Audit

Use this reference for every change to Socks Media Workflow, including instructions, references, scripts, templates, dependencies, connectors, or packaged releases.

## Required update record

After applying a change and before calling the update complete, create a new versioned Markdown audit. Never overwrite or silently replace an earlier audit.

Record:

- skill version, audit date, and change scope;
- files or capabilities added, changed, or removed;
- validation performed and its result;
- tested evidence, untested claims, and known failure cases;
- capability level for each affected workflow area;
- data, connector, authorization, and human-approval dependencies;
- actions the skill can analyze or draft but cannot execute;
- regressions, unresolved gaps, and recommended next priorities;
- comparison with the preceding retained audit.

Use these capability labels consistently:

- **Mature:** explicit workflow, evidence rules, error handling, and validated output behavior exist.
- **Usable:** reliably supportable when required inputs or tools are available.
- **Early:** partial reasoning or drafting support exists, but dedicated rules or validation are incomplete.
- **Not implemented:** the skill does not contain a sufficient method for the capability.
- **Execution prohibited:** analysis or approval-ready preparation may be possible, but the skill must not cause the live or external action.

Do not convert labels into unsupported precision. Any percentage is a qualitative coverage estimate unless a defined evaluation set and measured pass rate are cited.

## Storage and naming

Use a filename that preserves chronological history, for example:

`Socks_Media_Workflow_v0.3_capability_audit_YYYY-MM-DD.md`

Save the user-facing audit as a persistent artifact when persistent file storage is available. Keep raw client data, private messages, recipient addresses, account identifiers, and confidential campaign values out of reusable audit files unless the user explicitly requests and authorizes their inclusion.

## Completion gate

Do not describe an update as complete until:

1. the skill passes structural validation;
2. changed behavior receives a relevant behavioral check when feasible;
3. the new capability audit is saved successfully;
4. the report distinguishes skill logic from connector access and execution authority;
5. unresolved limitations and untested areas remain visible.

After saving the skill, re-read the installed entrypoint and verify that it links this reference. A local edit, local validation, or package build alone does not prove that the installed skill was updated.

If persistent saving or installed-version verification fails, report that the update is not fully archived or active. Provide a recoverable local copy without claiming the retention requirement was met.
