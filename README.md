# CS 117: Project in Computer Vision (UC Irvine, Fall 2026)

Course website, served at https://jhoffman.github.io/cs117-fa26/.
Plain Jekyll 4 with no theme; styles are ported from the homepage
(`jhoffman.github.io`, `css/style.css` and `css/header.css`) and share its token names.

## Updating content

| What | Where |
|---|---|
| Course name, lecture time/room, Canvas/Ed/Gradescope/slides links, staff email | `_config.yml` (an empty link shows "coming soon") |
| Lecture topics and readings | `_data/schedule.tsv`, with one row per class meeting and a `subheading` row per week. `type` can be `cancelled` or `finals`. |
| Problem sets and project milestones | `_data/assignments.yml`. This file feeds the Assignments page, the Project page's milestone table, and the Out/Due labels on the Schedule. Enter each date once, here. |
| Instructor and TA cards | `_data/staff.yml`, with photos in `assets/images/` |
| Policies and grading | `syllabus.md` |
| Project instructions | `project.html` |

Late work is accepted for `grace_days` (2) days after the due date, set in `_config.yml`. The last accepted day is calculated and shown on every assignment. To give one assignment a different window, set `late_until: YYYY-MM-DD` on it in `assignments.yml`; use `late_until: "none"` for in-class work.

An assignment moves from Upcoming to Past once its last accepted day is over. The deploy workflow rebuilds the site every day, so this happens without a push.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000/cs117-fa26/.

## Deploying

Every push to `main` builds and deploys the site through `.github/workflows/pages.yml`. In the repo, go to Settings > Pages and set Source to **GitHub Actions** (this only needs doing once).

## Accessibility (WCAG 2.1 AA)

The layout, colours and tables are built to meet AA. When editing:

- **Headings:** each page's `<h1>` comes from `title:` in the front matter. Start page content at `##` and don't skip levels.
- **Colours:** use `--color-link` for text links, not `--color-accent`. The accent blue is only 3.3:1 on white, so keep it for borders and fills.
- **Link text:** make it descriptive ("PS1 handout", not "here"), and add "(PDF)" to links that point to PDFs.
- **Status:** never show status with colour alone. Use the `.tag` labels.
- **Photos:** staff photos use `alt=""` because the name sits right next to them. Any other image needs real alt text.
- **Linked files:** slides, handouts and PDFs must be accessible too. Export tagged PDFs, and caption lecture videos.
- **Checking:** before the quarter, run an [axe](https://www.deque.com/axe/devtools/) or Lighthouse check on each page.
