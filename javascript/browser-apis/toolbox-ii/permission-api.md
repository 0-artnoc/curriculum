---
author: rosielowther

levels:

  - basic

  - advanced

  - medium

  - beginner

type: normal

category: feature
aspects:
  - introduction
  - new
  - workout

standards:
  javascript.browser-apis-device.3: 10

links:

  - '[developers.google.com](https://developers.google.com/web/updates/2015/04/permissions-api-for-the-web){website}'


---

# Permission API

---
## Content

The **Permission API** is a standard way to check the permission status of an API.

You can check the status of a permission using `permissions.query()`. The status is either **granted**, **denied** or **prompt** (if you need to request the permission from the user).

For example:

```
// Check for Geolocation API permissions.
// Pass permission's name into method
// as 'permissionDescriptor' object.
navigator.permissions
               .query({name:'geolocation'})
  // The Promise resolves to
  // `permissionStatus' object
  .then(function(permissionStatus) {
    // print state of geolocation permission
    console.log('geo permission
        state is ', permissionStatus.state);
  });
```
You can also create an event handler for `permissionStatus.onchange`.

Requesting permission from the user still depends on the specific API.

Currently this API is available in **Chrome** and **Firefox**.

---
## Practice

How do you check the status of a permission? ???

* `permissions.query();`
* `permissions.status();`
* `permissions.log();`
* `permission.status();`
* `permission.log();`
* `permission.query();`

---
## Revision

To what browsers is the Permission API currently limited to?
??? ???


* Chrome
* Firefox
* Safari
* Internet Explorer
 
