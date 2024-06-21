# Lighthouse v2 ![version](https://img.shields.io/static/v1.svg?label=v.&message=0.0.1&color=blue)

## A community project
Lighthouse is a journalling app designed by plural people, for plural people. Unlike most journalling methods, Lighthouse provides a **private journal** for each alter to use as their own space. But users can also process thoughts and feelings in the **communal journal** or in the **internal forum**.

The goal of Lighthouse is specifically for communication internally. No socialising will be implemented into the site.

## Development
### Stack
Lighthouse uses the **PEN** Stack- Postgres, Express, Node.js. Templating is done with EJS.

### Coding Standard
This is the standard for how Lighthouse v2 will be written:

- Keep all required modules at the top of the file. Order should be: NPM packages -> local files
- Keep related routes, middleware, etc in the same file. Example: `alter.js` should only have routes pertaining to alters.
- Variables and functions should be camelCased and pertain to the data they are assigned to. Examples: `selectedAlter`, `changeToDarkMode()`, `journalSkin`. This is for accessibility.
- Classes should be Proper Cased and pertain to the data they represent. Examples: `const alter = new Alter(name, id, pronouns); alter.loadInformation()`. This is for accessibility.
- Use JSDocs `/** */` to document functions. Comments should be used primarily for confusing code.
- Routes should have unit tests.
- Use #region comments to section off large chunks of code, such as separating post, get, put, and delete requests.