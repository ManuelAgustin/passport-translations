passport-translations
==============================================================================

[Short description of the addon.]


Compatibility
------------------------------------------------------------------------------

* Ember.js v3.16 or above
* Ember CLI v2.13 or above
* Node.js v10 or above


Installation
------------------------------------------------------------------------------

```
ember install passport-translations
```


Usage
------------------------------------------------------------------------------

[**Workflow**
- Check out this project locally and modify translation files in it
- `yarn link` in *passport-translations* folder (this will publish the local project for use by other local projects)
- `yarn link passport-translations` in *passport-frontend* folder: this will link that published version to be used instead of GitHub version
- after modifying files in *passport-translations*, make a PR in the translations repo
- after PR is merged and new version of *passport-translations* is released, update main project's `package.json` with the new version

**Workaround**
- by default all translations from the passport-translations addon are used
- but, if the main app has the same strings as the addon - the ones from main app take priority
So basically, the simplest way is:
- if you need to quickly modify/add translation strings — **override** them, by adding them to main app's translations/ folder (right now I deleted the folder, you can recreate)
- when a certain amount of overridden strings accumulates in the main app — we will dump them as a batch into translations project
- but in this case someone will have to carefully do the manual periodic dumping of those strings]


Contributing
------------------------------------------------------------------------------

See the [Contributing](CONTRIBUTING.md) guide for details.


License
------------------------------------------------------------------------------

This project is licensed under the [MIT License](LICENSE.md).
