# CodePath Contribution Report

## Reproduction Process

### Environment Setup

I set up the project locally from my fork of `angular/components`. One challenge I faced was that `pnpm` was not installed or available correctly in my environment, so the dependency install could not run at first. I solved this by installing/enabling `pnpm`, then I ran `pnpm i` and started the local dev app with `pnpm dev-app`.

### Steps to Reproduce

1. Run `pnpm dev-app`.
2. Open the dev app and navigate to `/list`.
3. Scroll to the `Single Selection list` section.
4. Hover over the radio indicator next to the disabled `Strawberries` option.
5. Observe that the cursor changes to a pointer even though the option is disabled.

### Reproduction Evidence

- **Branch link:** https://github.com/dipeshpandit12/components/tree/fix-button-disabled-state
- **Screenshots/logs:** I reproduced the issue locally in the list demo.
![alt text](IMG_8338.HEIC)
![alt text](IMG_8337.HEIC)
- **My findings:** The issue happens only in single-selection mode because it uses a radio-style indicator. The multiple-selection checkbox indicator already handles the disabled cursor correctly.
