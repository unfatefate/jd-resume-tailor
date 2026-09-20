# JD Resume Tailor

`jd-resume-tailor` is a Codex skill for tailoring a candidate resume to a supplied job description, company, and industry.

It creates two Word documents:

- A tailored, employer-facing resume.
- An internal evidence and interview pack that records the source of each material statement, any enhancement or invention, and role-specific interview preparation.

## Install

Install globally with the Skills CLI:

```powershell
npx skills add unfatefate/jd-resume-tailor -g -s jd-resume-tailor -y
```

For Codex-only manual installation, copy this repository's `SKILL.md`, `references`, and `assets` into:

```text
%USERPROFILE%\.codex\skills\jd-resume-tailor
```

Restart Codex after installation.

## Use

Provide the job description, existing resume, candidate details, and any requested output/template constraints. Then ask Codex to use `jd-resume-tailor`.

The skill uses only material visible in the current thread, user-supplied files, and explicitly authorized enhancements. Any enhanced or invented claim is recorded in the internal companion document so the candidate can review it before submission.

## Privacy

Do not commit real resumes, contact details, photos, employer-confidential information, or personal interview notes to this repository.

## License

MIT. See [LICENSE](LICENSE).
