# Animal Cell Culture Laboratory — Connected 3D Research Facility

A static, browser-based Three.js educational tour designed for a student presentation and deployment on Vercel.

## What's included

- **Zone 01 — Animal Cell Culture Suite:** ten selectable scientific equipment stations, ten clickable equipment worktables, two hand-wash basins, a shared sample-preparation table and four labelled waste bins.
- **Zone 02 — Instructor Chamber:** faculty mentoring, research-planning desk and meeting space.
- **Zone 03 — Research Students Chamber:** computer workstations and collaborative research space.
- **Zone 04 — Seminar & Discussion Hall:** presentation screen, stage and discussion seating.
- **Zone 05 — Lab Technician Chamber:** equipment records, inventory and operations support.
- **Zone 06 — Researcher Locker Room:** personal lockers, preparation bench and PPE storage point.
- A connected main corridor and cross-corridor, with an entry gate and an exit gate at opposite ends of the visitor route.
- Click-for-information hotspots for the rooms, room entrances, gates, corridor junctions, instruments, worktables, basins, waste bins, technician desk/counter, lockers, changing bench and PPE point.
- An opening welcome from **ANSHU YADAV — Research Fellow**, with a female voice preference and a bundled female narration fallback.
- 3D room navigation, camera orbit, zoom, keyboard movement and information panels.
- Real laboratory reference photographs from institutional pages, displayed with source attribution.
- Vercel static-site configuration. No server or build step is required.

## Run locally

The project is static. Open `index.html` in a modern browser, or use a local web server (recommended so browser features behave consistently):

```bash
# Windows PowerShell / Command Prompt
py -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy to Vercel

1. Extract the ZIP file.
2. Create a GitHub repository and upload the contents of this folder. `index.html` and `vercel.json` must be in the repository root.
3. Sign in to Vercel and choose **Add New → Project**.
4. Import the GitHub repository.
5. Select **Other** as the framework preset.
6. Leave Build Command and Install Command empty. Set Output Directory to `.`.
7. Deploy. Vercel will publish `index.html` as the site homepage.

You can also deploy with the Vercel CLI from this directory:

```bash
npm i -g vercel
vercel
```

## Controls

- Drag with mouse / finger: rotate the camera.
- Scroll / trackpad: zoom.
- W, A, S, D or arrow keys: move the camera target.
- Left-side navigation: fly to any of the six room zones.
- Select a glowing hotspot: open information about the selected room, fixture or equipment component.
- Audio buttons: play the welcome. The page selects an identifiable female English browser voice when available; otherwise it plays `welcome-female.mp3`.

## Important notes for the presentation

- The facility arrangement and room plan are an **illustrative academic concept**, not an official NIT Jalandhar architectural drawing or a claim about the institute's actual room allocation.
- ANSHU YADAV is presented as the virtual tour host because that name was provided for this assignment. The narration is synthetic and is not a recording of a real person.
- The browser's installed female English voice is preferred when one can be identified. The bundled fallback `welcome-female.mp3` was generated with the eSpeak TTS voice `en-us+f3` so a female voice is available when browser voices do not include one.
- The photographs are real reference images from the external institutional pages listed in `CREDITS.md`. They are not represented as photographs of NIT Jalandhar or as photographs of ANSHU YADAV.
- Three.js is loaded from a CDN, and reference photographs are loaded from their original web sources. An internet connection is therefore required when viewing the website. The bundled welcome audio is local to the project.
- Scientific operating details are educational summaries. Actual waste streams, gowning, emergency egress, access control, equipment use and biosafety practices must follow the institution's approved plans, current regulations, risk assessments and SOPs.
