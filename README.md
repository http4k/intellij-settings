# http4k IntelliJ Settings Repository

This repo contains a useful set of IntelliJ settings for use in http4k projects.

To add the repository to IntelliJ. The process requires temporarily disabling Settings Sync:

1. Disable `IntelliJ IDEA -> Settings -> Settings Sync`.
2. Open `IntelliJ IDEA -> Plugins` and search for and install `Settings Repository`. Restart.
3. Open `IntelliJ IDEA -> Settings -> Tools -> Settings Repository`
3. Hit `+` and add this repo: `https://github.com/http4k/intellij-settings`
4. Reenable `IntelliJ IDEA -> Settings -> Settings Sync`

### How to use the live templates

There are basically 4 types of template:

**to generate**|**shortcut + tab**|**result**|**example**
-----|-----|-----|-----
HttpHandler  | `hh`  | HttpHandler returning OK  | `{ req: Request -> Response(Status.OK) }`  
Filter | `fil`  | Empty filter |  `Filter { next -> { next(it) } }` 
Request | `get` etc  | Request for verb  |  `Request(Method.GET, "<URL>")`
Response | `200` etc  | Response with code  |  `Response(Status.OK)` 
