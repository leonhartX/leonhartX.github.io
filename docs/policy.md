---
layout: page
title: Privacy Policy
permalink: /policy/
---

## Personal data

### Crenditnal and user content for SCM service
Google Apps Script Github Assistant asks user's credential for the selected SCM service(Github/Github Enterprise/Bitbucket/GitLab)

The credential will be used to grant access token for selected SCM service and then discarded. The access token will be stored in browser's local storage through Web Storage API.

Google Apps Script Github Assistant will use the access token to get and update user's reporistory/branch/code in the selected SCM service when user perform the specific operations.

Google Apps Script Github Assistant had never and will never share any of above information to any others.

### Google login
Google Apps Script Github Assistant asks user to login with Google account. This is to grant permission for accessing Google Apps Script API to manage user's Apps Script code.

Google Apps Script Github Assistant only asks for the [script.projects](https://developers.google.com/identity/protocols/oauth2/scopes#script) scope

The oauth token grant through [chrome.identity](https://developer.chrome.com/docs/extensions/reference/identity/) and won't be stored directly anywhere

## Third party services
Google Apps Script Github Assistant uses:
- browser's Web Storage API (localStorage) for storing user's settings.
- GitHub API to access repository/branch/code information in GitHub or GitHub Enterprise.
- Bitbucket API to access repository/branch/code information in Bitbucket.
- GitLab API to access repository/branch/code information in GitLab.

Updated: Jan 4, 2021