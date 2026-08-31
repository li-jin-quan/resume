# Maintenance

Notes for the repository owner — not part of the public-facing resume.

## Regenerate the public PDF

The public PDF is generated from the redacted source script:

```bash
python D:/jl/gen_resume_public_pdf.py
```

Then push:

```bash
git push origin main
```

## Workflow (two-version policy)

1. Edit `D:/jl/gen_recruit_from_our_pdf.py` → regenerate the internal (headhunter-template) content version.
2. Run `D:/jl/gen_resume_public_pdf.py` → regenerate this public redacted PDF.
3. Commit and push both to keep them in sync.

> The public version redacts: phone number, original email, internal headhunter footer/branding, and any certifications not actually held.
