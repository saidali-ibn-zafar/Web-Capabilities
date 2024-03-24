# Permissions and Security

- Some permissions :

  - Are harmless

  - Have no cost

- Some other permissions :

  - Open a privacy risk

  - involves a cost

- When there are costs or risks, some browsers decide to put a limit on it:

  - User engagement requirements

  - Permission dialog to the user

- Most capabilities will require HTTPS

- Some Capabilities will need a user interaction to be enabled (aka you cannot trigger it on page load).

- Permissions are granted on an origin base

- If user denies a permission, the API won't be able to ask again, manual re-enable will be mandatory

- If user granted a permission, it may be with no time limit, for couple of days, for the session or just for one usage

---

![alt text](/imgSrc/image.png)

![alt text](/imgSrc/image-1.png)

---

`camera = \*` means any can access

`picture-in-picture = ()` is disabled

![alt text](/imgSrc/image-2.png)
