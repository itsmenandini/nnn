# UI refresh notes

This is a duplicate of the supplied TechAssures Lab project. The original upload was left unchanged.

## Changes in this pass
- The default appearance now stays light/white even when the Android device is set to dark mode, matching the approved reference screens.
- The in-app dark-mode theme remains available through the existing explicit theme toggle.
- The shared app header uses a white surface, no colored top border, no shadow, and only a subtle neutral bottom divider.
- Mobile page headings and page spacing were tightened slightly to better match the reference layout.

## Scope note
This pass is a source-level UI refinement, not a complete implementation of all 60 concept screens and not a compiled APK. Existing backend logic and role-specific access rules were not intentionally changed. The current test suites passed after these changes.

## Validation
Run `npm test` from the project root. Both the API and multi-lab tenancy suites passed when this duplicate was prepared.
