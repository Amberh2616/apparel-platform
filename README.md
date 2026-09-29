# ApparelTrack

AI-assisted product development and production software for the apparel industry.

## The problem

Garment development still runs on PDFs, spreadsheets and email. Every style
arrives as a tech pack, a bill of materials and a size spec — often in mixed
languages, inconsistent formats and changing across several sample rounds.
Teams re-key the same data by hand into production sheets, material lists and
cost sheets. It is slow, error-prone, and one person can realistically manage
only a few dozen styles a season.

## What ApparelTrack does

- **Reads development documents** — classifies tech pack pages and extracts
  bills of materials, size specs and construction notes, with a garment
  glossary of 1,200+ bilingual terms.
- **Turns them into structured, versioned data** — every sample round keeps its
  own immutable snapshot, so nothing is silently overwritten.
- **Runs the sample workflow** — sample requests, production work orders (PDF
  export), status tracking and a kanban board.
- **Engineering calculations** — pattern checking, fabric and thread
  consumption, and labour time, feeding into costing.
- **Downstream operations** — bulk orders, material requirements and purchase
  orders.

## How it is built

- **Traceable by design** — every number points back to the document, page and
  version it came from. Missing data is shown as missing, never guessed or
  filled with defaults.
- **Human in the loop** — AI proposes; people review and approve at each gate.
  Approved records are immutable.
- **Measured, not declared** — geometric values are measured from the actual
  drawn geometry, not copied from input parameters.

## Tech stack

Django · Django REST Framework · PostgreSQL · Celery/Redis ·
Next.js 14 · React · TypeScript · Python geometry engine · OpenAI vision models

## Status

In active private development. The source code is not public.
A demo is available on request.

---

Copyright © 2026 Amberh2616. All rights reserved.
No part of this project may be used, copied, modified or distributed
without written permission.
