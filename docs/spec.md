# Google Go style — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates it in CI. The prose headings are hand-owned — everything between `tl:*` markers is injected from the YAML items, so the published spec can never drift from the graph.

This source re-expresses the **Google Go Style Guide** as a grounded IDD graph: each major section is a `user_requirement`, and every individual rule is a `system_requirement` that `implements` its section. The guide reference lives in `attrs.source_ref`; the throughline UIDs are this source's own and immutable — a consumer cites a rule as `go:SR-0001`, never by section name.

It carries
<!-- tl:count type == 'user_requirement' -->
9
<!-- tl:end --> sections and
<!-- tl:count type == 'system_requirement' -->
64
<!-- tl:end --> style rules.

## Purpose

<!-- tl:item INT-0001 -->
**INT-0001 — Go is written in one clear, simple, consistent style** — `intent`, status `approved`

> The Google Go Style Guide exists so that Go across a large codebase reads as though written by one author: prioritising clarity of purpose and rationale, simplicity over cleverness, concision, and long-term maintainability, and staying consistent with idiomatic Go and the surrounding package so that any engineer can read and change code they did not write.

**source_ref**: Google Go Style Guide
<!-- tl:end -->

## Core Principles

<!-- tl:item UR-0001 -->
**UR-0001 — Core Principles** — `user_requirement`, status `approved`

> The overarching principles the guide optimises for and the baseline formatting expectations.

*Derives from:* INT-0001

**source_ref**: Google Go Style Guide: Core Principles
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Go Style Guide: Core Principles') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | approved | Make the code's purpose and rationale clear |
| SR-0002 | system_requirement | approved | Achieve goals in the most straightforward way |
| SR-0003 | system_requirement | approved | Keep a high signal-to-noise ratio |
| SR-0004 | system_requirement | approved | Design for change, not just for writing |
| SR-0005 | system_requirement | approved | Stay consistent with the surrounding codebase |
| SR-0006 | system_requirement | approved | Conform all files to gofmt |
| SR-0007 | system_requirement | approved | Do not impose a fixed maximum line length |
| SR-0008 | system_requirement | approved | Prefer local consistency unless it worsens a deviation |
<!-- tl:end -->

## Naming

<!-- tl:item UR-0002 -->
**UR-0002 — Naming** — `user_requirement`, status `approved`

> Rules governing the casing and choice of identifiers, receivers, packages, constants and initialisms.

*Derives from:* INT-0001

**source_ref**: Google Go Style Guide: Naming
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Go Style Guide: Naming') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0009 | system_requirement | approved | Use MixedCaps, not underscores |
| SR-0010 | system_requirement | approved | Do not use underscores in identifiers |
| SR-0011 | system_requirement | approved | Keep package names concise and lowercase |
| SR-0012 | system_requirement | approved | Use short, consistent receiver names |
| SR-0013 | system_requirement | approved | Name constants in MixedCaps by role |
| SR-0014 | system_requirement | approved | Case initialisms consistently |
| SR-0015 | system_requirement | approved | Avoid Get prefixes on getters |
| SR-0016 | system_requirement | approved | Match name length to scope |
| SR-0017 | system_requirement | approved | Reserve single-letter names for small scopes |
| SR-0018 | system_requirement | approved | Eliminate repetition in names |
<!-- tl:end -->

## Commentary

<!-- tl:item UR-0003 -->
**UR-0003 — Commentary** — `user_requirement`, status `approved`

> Rules governing doc comments, comment sentences, examples and package comments.

*Derives from:* INT-0001

**source_ref**: Google Go Style Guide: Commentary
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Go Style Guide: Commentary') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0019 | system_requirement | approved | Do not fix a comment line length |
| SR-0020 | system_requirement | approved | Give exported and non-obvious declarations doc comments |
| SR-0021 | system_requirement | approved | Write doc comments as complete sentences |
| SR-0022 | system_requirement | approved | Provide runnable examples in test files |
| SR-0023 | system_requirement | approved | Name result parameters only when they aid clarity |
| SR-0024 | system_requirement | approved | Place the package comment directly above the package clause |
<!-- tl:end -->

## Imports

<!-- tl:item UR-0004 -->
**UR-0004 — Imports** — `user_requirement`, status `approved`

> Rules governing import renaming, grouping, blank and dot imports.

*Derives from:* INT-0001

**source_ref**: Google Go Style Guide: Imports
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Go Style Guide: Imports') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0025 | system_requirement | approved | Do not rename imports without cause |
| SR-0026 | system_requirement | approved | Group imports in the standard order |
| SR-0027 | system_requirement | approved | Restrict blank imports to main and tests |
| SR-0028 | system_requirement | approved | Never use dot imports |
<!-- tl:end -->

## Errors

<!-- tl:item UR-0005 -->
**UR-0005 — Errors** — `user_requirement`, status `approved`

> Rules governing how errors are returned, phrased, handled and signalled.

*Derives from:* INT-0001

**source_ref**: Google Go Style Guide: Errors
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Go Style Guide: Errors') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0029 | system_requirement | approved | Return errors as the final result |
| SR-0030 | system_requirement | approved | Do not capitalise or punctuate error strings |
| SR-0031 | system_requirement | approved | Make a deliberate choice for every error |
| SR-0032 | system_requirement | approved | Signal failure with an error, not an in-band value |
| SR-0033 | system_requirement | approved | Handle the error first and unindent the happy path |
<!-- tl:end -->

## Language Features

<!-- tl:item UR-0006 -->
**UR-0006 — Language Features** — `user_requirement`, status `approved`

> Rules governing use of Go language features: panics, interfaces, generics, receivers, contexts and more.

*Derives from:* INT-0001

**source_ref**: Google Go Style Guide: Language Features
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Go Style Guide: Language Features') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0034 | system_requirement | approved | Do not panic for ordinary errors |
| SR-0035 | system_requirement | approved | Call Must functions only at startup |
| SR-0036 | system_requirement | approved | Make goroutine exit conditions explicit |
| SR-0037 | system_requirement | approved | Define interfaces where they are consumed |
| SR-0038 | system_requirement | approved | Use generics only to meet a real requirement |
| SR-0039 | system_requirement | approved | Pass small values, point at large ones |
| SR-0040 | system_requirement | approved | Choose the receiver type deliberately |
| SR-0041 | system_requirement | approved | Do not copy synchronisation objects |
| SR-0042 | system_requirement | approved | Omit redundant break in a switch |
| SR-0043 | system_requirement | approved | Prefer synchronous functions |
| SR-0044 | system_requirement | approved | Prefer type definitions to type aliases |
| SR-0045 | system_requirement | approved | Use %q to quote strings |
| SR-0046 | system_requirement | approved | Prefer any to interface{} |
| SR-0047 | system_requirement | approved | Do not define custom context types |
<!-- tl:end -->

## Formatting

<!-- tl:item UR-0007 -->
**UR-0007 — Formatting** — `user_requirement`, status `approved`

> Rules governing composite literals, function signatures, conditionals and layout beyond gofmt.

*Derives from:* INT-0001

**source_ref**: Google Go Style Guide: Formatting
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Go Style Guide: Formatting') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0048 | system_requirement | approved | Use composite literal syntax with clear field names |
| SR-0049 | system_requirement | approved | Name struct-literal fields for external types |
| SR-0050 | system_requirement | approved | Omit repeated element type names in literals |
| SR-0051 | system_requirement | approved | Omit zero-value fields where clarity allows |
| SR-0052 | system_requirement | approved | Prefer nil to an empty slice |
| SR-0053 | system_requirement | approved | Keep a function signature on one line |
| SR-0054 | system_requirement | approved | Do not line-break conditionals; extract operands |
| SR-0055 | system_requirement | approved | Separate awkward continuations with whitespace |
<!-- tl:end -->

## Common Libraries

<!-- tl:item UR-0008 -->
**UR-0008 — Common Libraries** — `user_requirement`, status `approved`

> Rules governing use of standard and Google libraries for flags, logging and randomness.

*Derives from:* INT-0001

**source_ref**: Google Go Style Guide: Common Libraries
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Go Style Guide: Common Libraries') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0056 | system_requirement | approved | Name flags snake_case and define them in main |
| SR-0057 | system_requirement | approved | Use the standard logging package appropriately |
| SR-0058 | system_requirement | approved | Use crypto/rand for cryptographic randomness |
<!-- tl:end -->

## Test Failures

<!-- tl:item UR-0009 -->
**UR-0009 — Test Failures** — `user_requirement`, status `approved`

> Rules governing how tests are written and how failures are reported.

*Derives from:* INT-0001

**source_ref**: Google Go Style Guide: Test Failures
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref', '').startswith('Google Go Style Guide: Test Failures') -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0059 | system_requirement | approved | Do not build assertion libraries |
| SR-0060 | system_requirement | approved | Identify the function and inputs in a failure |
| SR-0061 | system_requirement | approved | Print got before want |
| SR-0062 | system_requirement | approved | Compare whole structures |
| SR-0063 | system_requirement | approved | Prefer t.Error so a test keeps going |
| SR-0064 | system_requirement | approved | Compare with cmp.Equal and cmp.Diff |
<!-- tl:end -->

