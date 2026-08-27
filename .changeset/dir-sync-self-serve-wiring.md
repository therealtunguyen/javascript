---
'@clerk/clerk-js': minor
'@clerk/localizations': minor
'@clerk/shared': minor
'@clerk/ui': minor
---

Add self-serve Directory Sync (SCIM) setup. The `Organization` resource gains `getDirectorySync()`, `createDirectorySync()`, `updateDirectorySync()`, `rotateDirectorySyncToken()`, `deleteDirectorySync()`, and `getDirectorySyncUsers()` for managing the directory bound to an enterprise connection; the SCIM bearer token is only returned by create and rotate. The `OrganizationProfile` Security page gains a Directory Sync section, and the internal `ConfigureDirectorySync` component walks through the setup. Both are only shown when the instance has self-serve Directory Sync enabled.
