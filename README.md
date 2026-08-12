# Biomechanics Physical Screen

A single-file web app for running a non-clinical biomechanics physical screen —
standing posture with annotated body diagrams, dynamic movement (knee drive,
single-leg squat), toe touch, hip mobility and special tests, pelvic rotation,
foot & ankle measures, and cervical / upper-extremity range of motion. Generates
a printable client report with an automatic Problem List and signature block.

Built for BuildYou bike fitting. Everything lives in `index.html` — the body
diagram images are embedded, so there is nothing to install and no build step.

## Run it locally

Open `index.html` in any modern browser. That's it.

## Deploy on Vercel

1. Push this repository to GitHub (see below).
2. Go to [vercel.com/new](https://vercel.com/new) and import the repository.
3. Leave every setting as-is (Framework Preset: **Other**, no build command).
4. Click **Deploy**. Your screen will be live at `https://<project>.vercel.app`.

## Push to GitHub

Create an empty repository at [github.com/new](https://github.com/new), then:

```bash
git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

Or skip the command line: on your new empty GitHub repo page, choose
**"uploading an existing file"**, drag in `index.html` and `README.md`,
and commit.

## Notes

- Data entered into the form is saved in the browser (localStorage) so an
  accidental reload mid-screen doesn't lose work. The **Clear** button wipes
  it for the next client.
- Use **Preview Report → Save as PDF / Print** to produce the signed client
  record.
