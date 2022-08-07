# Vue ref bug

Steps to reproduce:

- Install deps
- `yarn dev`
- Go on site, open console
- Click the "Log ref content" button
- Two thing are logged, proxy of ref and validate method on of referenced component
- Stop dev server
- `yarn build`
- `yarn preview`
- Go on site, open console
- Click the "Log ref content" button
- Two thing are logged, proxy of ref and an undefined value which should be the referenced component validate method (here is the bug)
