# MEDical Image Computing Lab (MEDIC)

Official website for the Medical Image Computing Lab at UAEU.

🌐 **Live Site:** [https://damseh.github.io](https://damseh.github.io)

---

## About

This is the source code for the Medical Image Computing Lab website, led by Dr. Rafat Damseh at UAEU. Our research focuses on:

- AI and Machine Learning for Medical Imaging
- Cancer Diagnostics using Deep Learning
- Cerebrovascular Network Modeling
- Brain Connectivity Analysis
- Computer-Aided Diagnostic Systems

---

## Technology Stack

- **Static Site Generator:** Jekyll 3.8.5
- **Framework:** Bootstrap 3
- **Hosting:** GitHub Pages
- **Theme:** Custom research lab template

---

## Local Development

### Prerequisites

- Ruby 2.7 or higher
- Bundler
- Jekyll

### Setup

```bash
# Clone the repository
git clone https://github.com/Damseh/damseh.github.io.git
cd damseh.github.io

# Install dependencies
bundle install

# Run local server
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`

---

## Project Structure

```
damseh.github.io/
├── _config.yml              # Site configuration
├── _data/
│   ├── news.yml            # Lab news and updates
│   └── publications.json   # Publications list
├── _includes/              # Reusable HTML components
├── _layouts/               # Page layouts
│   ├── default.html
│   ├── homelay.html
│   └── member.html
├── _pages/
│   ├── home.md            # Homepage
│   ├── research.md        # Research areas
│   ├── publications.html  # Publications page
│   ├── news.html          # News page
│   ├── openings.md        # Open positions
│   └── team/              # Team member profiles
├── images/                # Images and media
│   ├── team/             # Team member photos
│   └── logo/             # Lab logo
└── css/                   # Stylesheets
```

---

## Adding Content

### Adding a Team Member

Create a new file in `_pages/team/_posts/` with the format `YYYY-MM-DD-firstname-lastname.md`:

```markdown
---
layout: member
category: graduate  # or 'staff'
title: Full Name
image: filename.jpg
role: PhD Student
permalink: 'team/firstname-lastname'
social:
    github: https://github.com/username
    google-scholar: https://scholar.google.com/...
education:
 - Degree, University, Year
---

Brief bio paragraph here.
```

Add their photo to `images/team/filename.jpg`

### Adding a Publication

Add to `_data/publications.json`:

```json
{
  "id": "unique_id",
  "type": "article-journal",
  "title": "Paper Title",
  "container-title": "Journal Name",
  "volume": "XX",
  "DOI": "10.xxxx/xxxxx",
  "author": [
    {"family": "LastName", "given": "FirstName"}
  ],
  "issued": {"date-parts": [["YYYY", "MM"]]}
}
```

### Adding News

Add to `_data/news.yml`:

```yaml
- date: DD/MM/YYYY
  title: "News Title"
  tags: [publication, grant, award]
  content: "Description of the news"
```

---

## Deployment

The site automatically deploys to GitHub Pages when you push to the `main` branch:

```bash
git add .
git commit -m "Update content"
git push origin main
```

Changes will be live at https://damseh.github.io within 2-3 minutes.

---

## Open Source Tools

Our lab develops and maintains several open-source projects:

- **[VascGraph](https://github.com/Damseh/VascularGraph)** - Vascular network segmentation and analysis
- **[VirtualMRI](https://github.com/Damseh/virtualMRI)** - Monte Carlo MRI simulation
- **[AngioPulse](https://github.com/Damseh/angiopulse)** - Pulsatile flow dynamics simulation

---

## Contact

**Dr. Rafat Damseh**  
Associate Professor  
Department of Computer Science and Software Engineering  
UAEU  
📧 rdamseh@uaeu.ac.ae  
🏢 Room 3070, P.O. Box 15551, Al Ain, UAE

---

## Credits

Website template adapted from the [Allan Lab](https://github.com/mpa139/allanlab) Jekyll theme for research groups.

---

## License

Content © 2021-2025 Medical Image Computing Lab, UAEU.  
Website code licensed under MIT License.
