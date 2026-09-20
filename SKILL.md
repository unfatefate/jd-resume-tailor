---
name: jd-resume-tailor
description: "Tailor a candidate resume to a supplied job description, company, and industry, then create a traceable Word resume plus an internal Word evidence and interview pack."
---

# JD Resume Tailor

Use when a user supplies a JD, job/company target, current resume, and candidate details and asks for a tailored resume. Inputs may be chat text, screenshots, links, PDF, Word, or images.

## Scope

- Build a temporary candidate evidence pool from the current user request, attached materials, and history visible in the current thread.
- Do not assume knowledge from another thread or history that is not visible. Ask for needed facts again.
- Read `references/jd-and-industry-analysis.md`, `references/evidence-and-claims.md`, and `references/rewrite-depth.md` before drafting.
- Read `references/traceability-and-interview-pack.md` before creating the internal attachment.
- Use the `docx` and `documents` skills for Word editing and render verification.

## Workflow

1. Inspect the existing resume and identify the user's template, fixed sections, photos, layout constraints, and requested output location.
2. Extract the JD into responsibilities, requirements, skills, metrics, company context, and industry language. Research public company/industry information when it materially improves relevance.
3. Build a `JD requirement -> candidate evidence -> rewrite strategy` map. Do not force coverage where there is no relevant evidence or user-authorized invention.
4. Classify every key claim as `original_fact`, `reasonable_extension`, `enhanced_expression`, or `invented_content`.
5. Select the rewrite depth from the JD gap. Preserve effective content and rewrite the modules that determine fit; do not mechanically rewrite every sentence or merely swap keywords.
6. Create the tailored resume. Preserve the supplied Word template unless the user explicitly asks for a new design. Use concise, concrete, role-appropriate bullets and keep any user-supplied quantitative claims intact.
7. Create the companion Word file using `assets/traceability-and-interview-pack-template.docx` as the starting structure. It is for the user's internal review only, never a document to submit to an employer.
8. Render and inspect every generated Word file. Verify page count, text overflow, photos, tables, alignment, legibility, dates, companies, numbers, and repeated wording.

## Claim Rules

- Respect the user's stated allowance for enhancement or invention, but record every non-original claim in the companion document.
- Never present a new numeric result as source-backed. Record its basis and classification in the companion document.
- Use company and industry research to choose wording, priorities, and plausible operating context. Do not silently turn industry norms into candidate facts.
- Preserve the distinction between source facts, extensions, enhancements, and inventions in the companion document even if the resume itself uses stronger positioning.

## Deliverables

Create at least two Word files in the user-selected directory:

- `岗位名称_姓名_简历.docx`
- `岗位名称_姓名_简历溯源与面试准备.docx`

If no output location is supplied, use the input resume's directory or the current workspace. Give both final files to the user and summarize the targeting decisions and any high-risk claims.

## Reference Routing

- JD/company/industry extraction: `references/jd-and-industry-analysis.md`
- Claim classification and source ledger: `references/evidence-and-claims.md`
- How much to rewrite: `references/rewrite-depth.md`
- Internal attachment fields and interview preparation: `references/traceability-and-interview-pack.md`
