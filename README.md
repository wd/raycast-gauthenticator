## Raycast Gauth

This is a tow-factor code generate extension for raycast, it works just like the Google Authenticator or other Two-Factors Authenticators.

This extension is compact with the [alfred-workflow-gauth](https://github.com/moul/alfred-workflow-gauth), so that it can reuse the configuration file.

## Configure

Create a `~/.gauth` file with your secrets.

```
[google - bob@gmail]
secret=xxxxxxxxxxxxxxxxxx

[evernote - robert]
secret=yyyyyyyyyyyyyyyyyy
```

⚠️ Note:
- Please **DO NOT** add `.` in the section name, because that will create a [subsction](https://en.wikipedia.org/wiki/INI_file#Hierarchy_(section_nesting)) which is not suppported by this extension. 
- Store your 2fa secret in a plain text on the file system might be a bit insecure. Please use with caution.

## Install

``` shell
brew install npm
npm install
npm run dev
```

It will open raycast and install the extension automatically after the last command.

## Thanks

* The `src/totp.ts` were stolen from the `two-factor-authentication-code-generator`, thanks to the author.
