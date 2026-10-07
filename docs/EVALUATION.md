# Birdkanfly — Evaluation guide

Start with the smallest path that exercises the project. Distinguish source inspection,
syntax/build checks, functional behavior and domain validation when recording a result.

## Guided reading and demonstration

1. **Explore the academy.** Start on the landing page and follow the academy, program and fleet
links. The page content is authored in Astro source.

2. **Compare pathways.** Open Programs and Admissions to inspect the course and application copy.
Validate dates and requirements with the academy before publication.

3. **Inspect the fleet.** Use the fleet page as a presentation of supplied content, not an
independent airworthiness or availability record.

4. **Make an enquiry.** Review the contact page and its form behavior. A rendered enquiry form is
separate from proof that a message reaches an operational inbox.

## Declared checks

These commands/checks describe the intended verification path. Their presence in this
guide does not claim that they passed. See the dated evidence below and the README for setup.

```text
npm run build
```

## Evidence levels

| Level | What it establishes | What it does not establish |
| --- | --- | --- |
| Source review | A path exists in tracked code | Successful runtime behavior |
| Syntax/build | Parser/compiler accepts that path | End-to-end correctness |
| Behavioral check | A specific input/output case passed | Generalization beyond cases |
| Domain evaluation | Performance on a stated target setting | Other users/data/environments |

## What to record

- Commit, environment, dependency versions and date.
- Input provenance and whether data is synthetic, public or privately supplied.
- Absolute pass/fail/skip counts; keep failed cases and their root causes.
- Whether external services, hardware or a production deployment were actually exercised.
- Expected output and an artifact showing the observation.

## Review scenarios

- **Pages rather than one long form:** Training, aircraft and admissions have distinct reading
tasks.

- **Shared shell:** The layout/header/footer provide consistency across routes.

- **Business claims remain attributable:** The source contains marketing statements; documentation
does not certify them.

## Documentation inspection — 7 October 2026

The documentation was traced to committed source and checked for local links, balanced
code fences and supported implementation claims. Historical notebook outputs remain labeled
as historical. Live provider access, private databases and hardware behavior are not inferred
from configuration or dependency files. Any fresh run is recorded separately in the README.

## Next evidence to collect

- Validate academy copy and accreditation references.
- Test every navigation and contact action.
- Record a production build and mobile acceptance run.

## Fresh checks

The README records fresh checks on 7 October 2026, including commands and absolute results.
Those measured checks supersede an inspection-only description for the paths they cover.
