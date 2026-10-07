# Birdkanfly — Architecture and implementation

This guide follows the tracked implementation. Proposed work is identified separately.

## The problem and the system boundary

Prospective pilots need to understand training pathways, aircraft and admission requirements
before contacting an academy. The site organizes that information into dedicated pages, with
shared navigation and a consistent academy presentation.

## Processing path

```mermaid
flowchart LR
    N0["Astro pages"]
    N1["Shared layout"]
    N2["Static build"]
    N3["Visitor enquiry"]
    N0 --> N1
    N1 --> N2
    N2 --> N3
```

## End-to-end behavior

### 1. Explore the academy

Start on the landing page and follow the academy, program and fleet links. The page content is
authored in Astro source.

### 2. Compare pathways

Open Programs and Admissions to inspect the course and application copy. Validate dates and
requirements with the academy before publication.

### 3. Inspect the fleet

Use the fleet page as a presentation of supplied content, not an independent airworthiness or
availability record.

### 4. Make an enquiry

Review the contact page and its form behavior. A rendered enquiry form is separate from proof that
a message reaches an operational inbox.

## Design choices and consequences

### Pages rather than one long form

Training, aircraft and admissions have distinct reading tasks.

### Shared shell

The layout/header/footer provide consistency across routes.

### Business claims remain attributable

The source contains marketing statements; documentation does not certify them.

## Source entry points

### [src/pages/index.astro](../src/pages/index.astro)

This file is part of the reviewed path described above. Follow its imports and calls
for the exact interface rather than inferring behavior from the filename.

### [src/pages/programs.astro](../src/pages/programs.astro)

This file is part of the reviewed path described above. Follow its imports and calls
for the exact interface rather than inferring behavior from the filename.

### [src/pages/admissions.astro](../src/pages/admissions.astro)

This file is part of the reviewed path described above. Follow its imports and calls
for the exact interface rather than inferring behavior from the filename.

### [src/pages/contact.astro](../src/pages/contact.astro)

This file is part of the reviewed path described above. Follow its imports and calls
for the exact interface rather than inferring behavior from the filename.

### [src/layouts/Layout.astro](../src/layouts/Layout.astro)

This file is part of the reviewed path described above. Follow its imports and calls
for the exact interface rather than inferring behavior from the filename.

## Implementation state

| State | Evidence boundary |
| --- | --- |
| Present | Six authored pages and shared header/footer |
| Present | Responsive styles and animation dependencies |
| Needs verification | Business claims, course dates and contact details |
| Not verified | Enquiry delivery and live hosting |

“Present” means tracked source or assets exist. It does not mean a production or domain
validation has passed. See [Evaluation](EVALUATION.md) for reproducible checks and limits.
