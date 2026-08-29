---
'@clerk/nextjs': patch
---

Fixed a spurious "Each child in a list should have a unique key prop" React warning logged in development from `<ClerkProvider>` in the App Router, e.g. when passing a large `localization` object. The warning pointed at an unrelated internal component and did not indicate a real bug.
