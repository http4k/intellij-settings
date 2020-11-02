# http4k IntelliJ Settings Repository

This repo contains a useful set of IntelliJ settings for use in http4k projects.

To add the repository to IntelliJ:

1. Open `IntelliJ -> File -> Preferences -> Tools -> Settings Repository`
2. Hit `+` and add this repo: `https://github.com/http4k/intellij-settings`

### How to use the live templates

There are basically 4 types of template:

**to generate**|**shortcut + tab**|**result**|**example**
-----|-----|-----|-----
HttpHandler  | `hh`  | HttpHandler returning OK  | `{ req: Request -> Response(Status.OK) }`  
Filter | `fil`  | Empty filter |  `Filter { next -> { next(it) } }` 
Request | `get` etc  | Request for verb  |  `Request(Method.GET)`
Response | `200` etc  | Response with code  |  `Response(Status.OK)` 
