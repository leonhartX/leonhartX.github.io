---
layout: page
title: Privacy Policy
permalink: /policy/
---

## Personal data

### SCM(remote Git) services
Google Apps Script GitHub Assistant asks user's credential for the selected SCM service(Github/Github Enterprise/Bitbucket/GitLab)

The credential will be used to grant access token for selected SCM service and then discarded. The access token will be stored in browser's local storage through Web Storage API.

Google Apps Script Github Assistant will use the access token to get and update user's reporistory/branch/code in the selected SCM service when user perform the specific operations.

Google Apps Script Github Assistant had never and will never share any of above information to any others.

### Google
Google Apps Script Github Assistant asks user to login with Google account after user login to remote Git service. This is to grant permission for accessing Google Apps Script API to manage user's Apps Script code.

After user login, Google Apps Script Github Assistant will access to user's Apps Script project content under user's operation
  - when user clicking `Push` button in Apps Script Editor, Google Apps Script Github Assistant get the content of current Apps Script project and send to remote Git service.
  - when user clicking `Pull` button in Apps Script Editor, Google Apps Script Github Assistant get the content of remote Git Service and update them to current Apps Script project.

Google Apps Script Github Assistant won't store and share anything of user's Apps Script project. After the `Push` or `Pull` operation, all the contents fetched will be discarded.

Google Apps Script Github Assistant only asks for the [script.projects](https://developers.google.com/identity/protocols/oauth2/scopes#script) scope

The OAuth token grant through [chrome.identity](https://developer.chrome.com/docs/extensions/reference/identity/) and won't be stored directly anywhere




## Third party services
Google Apps Script Github Assistant uses:
- browser's Web Storage API (localStorage) for storing user's settings.
- GitHub API to access repository/branch/code information in GitHub or GitHub Enterprise.
- Bitbucket API to access repository/branch/code information in Bitbucket.
- GitLab API to access repository/branch/code information in GitLab.

Updated: Jan 4, 2021