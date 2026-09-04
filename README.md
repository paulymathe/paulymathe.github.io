# Paul Bastin — Hugo academic website

A minimal Hugo academic website inspired by the structure of AcademicPages / Minimal Mistakes: top navigation, profile sidebar, and a main content column.

## 1. Install Hugo

On Windows PowerShell:

```powershell
winget install Hugo.Hugo.Extended
```

Check:

```powershell
hugo version
```

## 2. Preview locally

From this directory:

```powershell
hugo server
```

Then open http://localhost:1313/

## 3. Customize

Edit `hugo.toml`:

- `baseURL`
- role / affiliation
- email
- GitHub / Scholar / HAL / arXiv / ORCID links
- profile image path

Replace `static/images/profile-placeholder.svg` with your photo, for example `static/images/profile.jpg`, then set:

```toml
avatar = '/images/profile.jpg'
```

Edit the Markdown pages under `content/`.

Put your CV at:

`static/files/cv.pdf`

## 4. GitHub Pages

Create a public GitHub repository named:

`YOUR-USERNAME.github.io`

Then set the correct `baseURL` in `hugo.toml`.

Push this project to the repository. On GitHub go to:

Settings → Pages → Source → GitHub Actions

The included `.github/workflows/hugo.yaml` will build and deploy the site after each push to `main`.
