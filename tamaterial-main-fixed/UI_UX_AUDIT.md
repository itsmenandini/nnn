# TechAssures Lab — UI/UX Consolidation

## Scope of this update
This pass updates the shared design system across the existing application routes. It does not create duplicate pages for every numbered concept mockup. Where the mockups show the same information in multiple screens (for example report preview/share, invoice detail/payment, and client/work-order details), the existing route and modal/drawer workflows remain the source of truth.

## Visual system applied
- White page headers with a subtle neutral divider; no thick green top border.
- White cards on a soft light-grey canvas, consistent border radius and restrained shadows.
- Deep green primary actions and active states; status colours remain semantically distinct.
- Standardized input, tab, badge, card, button and bottom-navigation sizing.
- Mobile breakpoints for narrow Android screens and larger tablet/desktop layouts.
- Safe-area spacing for bottom navigation and fixed action bars.
- Reduced-motion preference and horizontally scrollable wide report tables.

## Existing workflow surfaces covered by the shared UI pass
1. Login, Google sign-in, PIN recovery and lab onboarding.
2. Role dashboard, tasks and notifications.
3. Client list, client detail, projects, work orders, CRM and quotes.
4. New sample wizard, sample list/detail and test selection.
5. Testing schedule, job entry, measurements, photos and location evidence.
6. Review queue, validation, return/resubmit, approval and digital signature.
7. Report preview, PDF/QR and sharing.
8. Billing approval, rate book, invoices, payments and cheque lifecycle.
9. Admin user management, authorised tests/signatory controls, test master and settings.
10. Tickets/support, profile and audit/activity views where exposed by the existing app.

## Guardrails
- No new backend routes or database schema changes were made in this styling pass.
- Existing role-based access checks and business logic were left intact.
- Test-specific fields must continue to come from the configured test definitions; generic cube values in concept mockups are illustrative only.
- Deferred items in `DEFERRED.md` remain deferred unless separately implemented and tested.

## Verification
Run `npm test` from the project root. Visual verification should also be completed on a narrow Android device and a desktop browser before release. This is a source-code UI refresh, not a claim that a production APK has been compiled or device-tested.
