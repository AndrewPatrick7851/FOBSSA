# FOBSSA · Faculty of Biological Sciences Students’ Association

At Alex Ekwueme Federal University Ndufu-Alike (AE-FUNAI), FOBSSA brings together students across the Faculty of Biological Sciences. This repository documents a piece of my work in faculty leadership and software development. I served as Faculty Director of Action and Mobilization and coordinated Faculty Cultural Day. Through AndrewPatrick Technologies, I developed the FOBSSA Digital System to give students a place to find association services and to help organizers issue and verify certificates.

## What the digital system does

| For | Feature |
| --- | --- |
| Students | A responsive homepage brings together Quick Services, information about FOBSSA, and the faculty’s academic departments. |
| Event organizers | The certificate workflow uses records in Google Sheets and a Google Slides template to generate personalized certificates, export PDFs, and deliver them by email. |
| Certificate holders and reviewers | A QR code connects the certificate to a verification portal where a reviewer can check the record. |

The homepage is built with HTML, CSS, JavaScript, and Bootstrap. The certificate workflow runs in Google Apps Script. The implementation is in the private [FOBSSA Digital System repository](https://github.com/AndrewPatrick7851/FOBSSA-Digital-System). GitHub access is required to view or clone it.

## Getting started

This public overview can be read directly on GitHub. Contributors with access to the companion repository can preview the homepage locally.

1. Clone the companion repository and enter its directory.

   ```sh
   git clone https://github.com/AndrewPatrick7851/FOBSSA-Digital-System.git
   cd FOBSSA-Digital-System
   ```

2. Open `frontend/index.html` in a browser. The page loads Bootstrap from a CDN. The HTML currently references `css/style.css` and `js/app.js`, while the tracked files are at `css/css/style.css` and `js/js/app.js` under `frontend/`. Adjust those references in your local copy to preview the custom styling and script.

3. For the certificate workflow, review `backend/app-scripts/`, starting with `config.gs`. It defines the sheet name and column mapping, Slides template, output folders, and verification URL. **Maintainer input needed:** confirm the test resources, script execution order, and web app deployment settings before running an end-to-end test.

## Screenshots

| Planned view | Screenshot needed from the maintainer |
| --- | --- |
| Student homepage | Capture the Quick Services and Academic Departments sections. |
| Certificate and verification | Show a sample PDF and its matching portal result using a fictional recipient and demonstration record. |

*Developed by AndrewPatrick Technologies.*