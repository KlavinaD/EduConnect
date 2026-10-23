# EduConnect — React website

A new five-page version based on the supplied visual reference. The original project is unchanged.

## Open the website

Double-click `index.html`. The bundled React libraries make the interface work without an installation or build step. External learning materials still require internet access. For consistent reading-list storage across pages, use the local server below: browser restrictions can affect storage when opening local files directly.

For a local server, open a terminal in this folder and run:

```sh
python3 -m http.server 4173
```

Then visit http://localhost:4173. Stop the server with Ctrl+C.

## Folder structure

- `index.html`: convenient Home entry point.
- `html/`: Home, Resources Catalogue, Resource Details, My Reading List and About.
- `css/desktop/styles.css`: shared foundations and desktop layout.
- `css/mobile/styles.css`: tablet and mobile overrides.
- `javascripts/app.js`: React components and interaction logic, written with htm template literals rather than a JSX build step.
- `javascripts/resources.js`: resource data reused from the supplied project.
- `javascripts/vendor/`: locally bundled React 18.3.1, ReactDOM 18.3.1 and htm 3.1.1.
- `assets/`: existing project images and the new favicon.

## Included features

Subject browsing; keyword search; subject/level/format filters; A–Z / Z–A sorting; real pagination; resource details and keyboard-accessible tabs; provider links; related resources; save/remove reading-list items; saved count; clear-all with undo; empty states; responsive navigation; local storage with a fallback warning.

## Scope and content

There are no accounts, admin tools, upload forms or server database in this version. Learning materials remain on their provider websites; the Visit Resource action opens the provider. Direct downloading is not simulated or claimed. Some providers have paid certificates or account requirements, noted on the details page.

The supplied project contains 13 resources, not the 24 shown in the visual reference. No extra resources or test results were invented. Suggested learning-focus prompts are general guidance written for this prototype, not provider-certified outcomes. The source URLs and access notes are carried over from the supplied project and have not been independently rechecked in this revision.

The reading list uses the existing `educonnect-reading-list-v1` storage key, so saved IDs can be retained when served from the same origin. Different ports, domains or local-file policies may use different storage.

The React framework is included; Angular is not needed alongside it. No remote font or library CDN is required at runtime.

## Third-party libraries

React and ReactDOM are copyright Meta Platforms, Inc. and affiliates, MIT licensed. htm is copyright Jason Miller, Apache-2.0 licensed. See the license files in `javascripts/vendor/`.

Project source licensing should be agreed by the group before publishing it as open source. Provider materials have their own licenses.
