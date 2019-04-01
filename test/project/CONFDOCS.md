## Plugin [@blackflux/robo-config-plugin](https://www.npmjs.com/package/@blackflux/robo-config-plugin)

### >> `semantic-release/@default`

Recommended base configuration when using [semantic-release](https://github.com/semantic-release/semantic-release).

<!---0--><details>
<!---0--><summary>Targets</summary>

```
project
└─ .releaserc.json
```

<!---0--></details>

<!---0--><details>
<!---0--><summary>Requires</summary>

- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Details</summary>

#### >>> semantic-release/commit-conventions

_Updating `.releaserc.json` using `overwrite`._

- Slightly extended [release commit convention](https://github.com/semantic-release/semantic-release#commit-message-format) for semantic-release.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .releaserc.json
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)

<!---1--></details>

------

<!---0--></details>

### >> `npm/@default`

Recommended base configuration when using [npm](https://www.npmjs.com/).

<!---0--><details>
<!---0--><summary>Targets</summary>

```
project
└─ .npmignore
```

<!---0--></details>

<!---0--><details>
<!---0--><summary>Requires</summary>

- [npm](#blackfluxrobo-config-plugin-req-ref-npm)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Details</summary>

#### >>> npm/npmignore

_Updating `.npmignore` using `unique-top`._

- Inject comment into .npmignore explaining when to use it.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .npmignore
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [npm](#blackfluxrobo-config-plugin-req-ref-npm)

<!---1--></details>

------

<!---0--></details>

### >> `license/@MIT-npm`

Recommended base configuration when using MIT License with npm.

<!---0--><details>
<!---0--><summary>Targets</summary>

```
project
├─ LICENSE
└─ package.json
```

<!---0--></details>

<!---0--><details>
<!---0--><summary>Requires</summary>

- [npm](#blackfluxrobo-config-plugin-req-ref-npm)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Variables</summary>

- [ownerName](#blackfluxrobo-config-plugin-var-ref-ownername)
- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Details</summary>

#### >>> license/MIT-LICENSE

_Updating `LICENSE` using `overwrite`._

- Generate [MIT license](https://en.wikipedia.org/wiki/MIT_License) file.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ LICENSE
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [ownerName](#blackfluxrobo-config-plugin-var-ref-ownername)

<!---1--></details>

#### >>> license/MIT-npm

_Updating `package.json` using `merge-shallow`._

- Link MIT license file into [npm](https://www.npmjs.com/) configuration.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ package.json
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [npm](#blackfluxrobo-config-plugin-req-ref-npm)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [ownerName](#blackfluxrobo-config-plugin-var-ref-ownername)
- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---1--></details>

------

<!---0--></details>

### >> `jetbrains/@default`

Recommended base configuration when using Jetbrains.

<!---0--><details>
<!---0--><summary>Targets</summary>

```
project
└─ .idea
   └─ ${projectName}.iml
```

<!---0--></details>

<!---0--><details>
<!---0--><summary>Requires</summary>

- [jetbrains](#blackfluxrobo-config-plugin-req-ref-jetbrains)
- [nyc](#blackfluxrobo-config-plugin-req-ref-nyc)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Variables</summary>

- [projectName](#blackfluxrobo-config-plugin-var-ref-projectname)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Details</summary>

#### >>> jetbrains/exclude-coverage-folder

_Updating `.idea/${projectName}.iml` using `xml-merge`._

- Mark `coverage` Folder as excluded in Jetbrains.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .idea
   └─ ${projectName}.iml
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [jetbrains](#blackfluxrobo-config-plugin-req-ref-jetbrains)
- [nyc](#blackfluxrobo-config-plugin-req-ref-nyc)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [projectName](#blackfluxrobo-config-plugin-var-ref-projectname)

<!---1--></details>

------

<!---0--></details>

### >> `git/@default`

Recommended base configuration when using [git](https://en.wikipedia.org/wiki/Git).

<!---0--><details>
<!---0--><summary>Targets</summary>

```
project
└─ .gitignore
```

<!---0--></details>

<!---0--><details>
<!---0--><summary>Requires</summary>

- [git](#blackfluxrobo-config-plugin-req-ref-git)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Details</summary>

#### >>> git/gitignore

_Updating `.gitignore` using `unique-top`._

- Inject recommended entries into [gitignore file](https://help.github.com/en/articles/ignoring-files).
- Default ignores for JetBrains IDE.
- Default ignores for OSX
- Default ignores for NodeJs

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .gitignore
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [git](#blackfluxrobo-config-plugin-req-ref-git)

<!---1--></details>

------

<!---0--></details>

### >> `editor/@default`

Recommended base [code editor configuration](https://editorconfig.org/).

<!---0--><details>
<!---0--><summary>Targets</summary>

```
project
└─ .editorconfig
```

<!---0--></details>

<!---0--><details>
<!---0--><summary>Details</summary>

#### >>> editor/two-space

_Updating `.editorconfig` using `overwrite`._

- Two space line indentation.
- Set `lf` line endings.
- Set `utf8` encoding.
- Remove unnecessary whitespaces.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .editorconfig
```

<!---1--></details>

------

<!---0--></details>

### >> `dependabot/@default-js`

Recommended base [dependabot configuration](https://dependabot.com/) for javascript projects.

<!---0--><details>
<!---0--><summary>Targets</summary>

```
project
└─ .dependabot
   └─ config.yml
```

<!---0--></details>

<!---0--><details>
<!---0--><summary>Requires</summary>

- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)
- [github](#blackfluxrobo-config-plugin-req-ref-github)
- [javascript](#blackfluxrobo-config-plugin-req-ref-javascript)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Details</summary>

#### >>> dependabot/js-instant

_Updating `.dependabot/config.yml` using `overwrite`._

- Configure dependabot to instantly merge javascript dependency updates into the `dev` branch.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .dependabot
   └─ config.yml
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)
- [github](#blackfluxrobo-config-plugin-req-ref-github)
- [javascript](#blackfluxrobo-config-plugin-req-ref-javascript)

<!---1--></details>

------

<!---0--></details>

### >> `badges/@npm-opensource`

Display various badges in README.

<!---0--><details>
<!---0--><summary>Targets</summary>

```
project
└─ README.md
```

<!---0--></details>

<!---0--><details>
<!---0--><summary>Requires</summary>

- [js-gardener](#blackfluxrobo-config-plugin-req-ref-js-gardener)
- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)
- [npm-published](#blackfluxrobo-config-plugin-req-ref-npm-published)
- [david-dm](#blackfluxrobo-config-plugin-req-ref-david-dm)
- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)
- [coveralls](#blackfluxrobo-config-plugin-req-ref-coveralls)
- [circleci](#blackfluxrobo-config-plugin-req-ref-circleci)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Variables</summary>

- [packageName](#blackfluxrobo-config-plugin-var-ref-packagename)
- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Details</summary>

#### >>> badges/js-gardener

_Updating `README.md` using `merge-below-title`._

- Display [js-gardener](https://github.com/blackflux/js-gardener) badge in README.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ README.md
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [js-gardener](#blackfluxrobo-config-plugin-req-ref-js-gardener)

<!---1--></details>

#### >>> badges/semantic-release

_Updating `README.md` using `merge-below-title`._

- Display [semantic-release](https://github.com/semantic-release/semantic-release) badge in README.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ README.md
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)

<!---1--></details>

#### >>> badges/npm-downloads

_Updating `README.md` using `merge-below-title`._

- Display [npm downloads](https://www.npmjs.com/) badge in README.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ README.md
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [npm-published](#blackfluxrobo-config-plugin-req-ref-npm-published)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [packageName](#blackfluxrobo-config-plugin-var-ref-packagename)

<!---1--></details>

#### >>> badges/npm-status

_Updating `README.md` using `merge-below-title`._

- Display [npm status](https://www.npmjs.com/) badge in README.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ README.md
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [npm-published](#blackfluxrobo-config-plugin-req-ref-npm-published)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [packageName](#blackfluxrobo-config-plugin-var-ref-packagename)

<!---1--></details>

#### >>> badges/david-dm

_Updating `README.md` using `merge-below-title`._

- Display [david-dm.com](https://david-dm.org/) badge in README.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ README.md
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [david-dm](#blackfluxrobo-config-plugin-req-ref-david-dm)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---1--></details>

#### >>> badges/dependabot

_Updating `README.md` using `merge-below-title`._

- Display [dependabot](https://dependabot.com/) badge in README.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ README.md
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---1--></details>

#### >>> badges/coveralls

_Updating `README.md` using `merge-below-title`._

- Display [coveralls](https://coveralls.io/) badge in README.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ README.md
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [coveralls](#blackfluxrobo-config-plugin-req-ref-coveralls)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---1--></details>

#### >>> badges/circleci

_Updating `README.md` using `merge-below-title`._

- Display [circleci](https://circleci.com/) badge in README.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ README.md
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [circleci](#blackfluxrobo-config-plugin-req-ref-circleci)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---1--></details>

------

<!---0--></details>

### >> `assorted/@npm-opensource`

Manage various configuration files for an open source npm github repo.

<!---0--><details>
<!---0--><summary>Targets</summary>

```
project
├─ .circleci
│  └─ config.yml
├─ .dependabot
│  └─ config.yml
├─ .gally.json
├─ .gitignore
├─ .npmignore
├─ .releaserc.json
├─ LICENSE
├─ package.json
└─ README.md
```

<!---0--></details>

<!---0--><details>
<!---0--><summary>Requires</summary>

- [js-gardener](#blackfluxrobo-config-plugin-req-ref-js-gardener)
- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)
- [npm-published](#blackfluxrobo-config-plugin-req-ref-npm-published)
- [david-dm](#blackfluxrobo-config-plugin-req-ref-david-dm)
- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)
- [coveralls](#blackfluxrobo-config-plugin-req-ref-coveralls)
- [circleci](#blackfluxrobo-config-plugin-req-ref-circleci)
- [github](#blackfluxrobo-config-plugin-req-ref-github)
- [javascript](#blackfluxrobo-config-plugin-req-ref-javascript)
- [git](#blackfluxrobo-config-plugin-req-ref-git)
- [npm](#blackfluxrobo-config-plugin-req-ref-npm)
- [yarn](#blackfluxrobo-config-plugin-req-ref-yarn)
- [gally](#blackfluxrobo-config-plugin-req-ref-gally)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Variables</summary>

- [packageName](#blackfluxrobo-config-plugin-var-ref-packagename)
- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)
- [ownerName](#blackfluxrobo-config-plugin-var-ref-ownername)
- [owner](#blackfluxrobo-config-plugin-var-ref-owner)
- [mergeBot](#blackfluxrobo-config-plugin-var-ref-mergebot)

<!---0--></details>

<!---0--><details>
<!---0--><summary>Details</summary>

#### >>> `badges/@npm-opensource`

Display various badges in README.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ README.md
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [js-gardener](#blackfluxrobo-config-plugin-req-ref-js-gardener)
- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)
- [npm-published](#blackfluxrobo-config-plugin-req-ref-npm-published)
- [david-dm](#blackfluxrobo-config-plugin-req-ref-david-dm)
- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)
- [coveralls](#blackfluxrobo-config-plugin-req-ref-coveralls)
- [circleci](#blackfluxrobo-config-plugin-req-ref-circleci)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [packageName](#blackfluxrobo-config-plugin-var-ref-packagename)
- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Details</summary>

##### >>>> badges/js-gardener

_Updating `README.md` using `merge-below-title`._

- Display [js-gardener](https://github.com/blackflux/js-gardener) badge in README.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ README.md
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [js-gardener](#blackfluxrobo-config-plugin-req-ref-js-gardener)

<!---2--></details>

##### >>>> badges/semantic-release

_Updating `README.md` using `merge-below-title`._

- Display [semantic-release](https://github.com/semantic-release/semantic-release) badge in README.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ README.md
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)

<!---2--></details>

##### >>>> badges/npm-downloads

_Updating `README.md` using `merge-below-title`._

- Display [npm downloads](https://www.npmjs.com/) badge in README.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ README.md
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [npm-published](#blackfluxrobo-config-plugin-req-ref-npm-published)

<!---2--></details>

<!---2--><details>
<!---2--><summary>Variables</summary>

- [packageName](#blackfluxrobo-config-plugin-var-ref-packagename)

<!---2--></details>

##### >>>> badges/npm-status

_Updating `README.md` using `merge-below-title`._

- Display [npm status](https://www.npmjs.com/) badge in README.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ README.md
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [npm-published](#blackfluxrobo-config-plugin-req-ref-npm-published)

<!---2--></details>

<!---2--><details>
<!---2--><summary>Variables</summary>

- [packageName](#blackfluxrobo-config-plugin-var-ref-packagename)

<!---2--></details>

##### >>>> badges/david-dm

_Updating `README.md` using `merge-below-title`._

- Display [david-dm.com](https://david-dm.org/) badge in README.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ README.md
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [david-dm](#blackfluxrobo-config-plugin-req-ref-david-dm)

<!---2--></details>

<!---2--><details>
<!---2--><summary>Variables</summary>

- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---2--></details>

##### >>>> badges/dependabot

_Updating `README.md` using `merge-below-title`._

- Display [dependabot](https://dependabot.com/) badge in README.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ README.md
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)

<!---2--></details>

<!---2--><details>
<!---2--><summary>Variables</summary>

- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---2--></details>

##### >>>> badges/coveralls

_Updating `README.md` using `merge-below-title`._

- Display [coveralls](https://coveralls.io/) badge in README.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ README.md
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [coveralls](#blackfluxrobo-config-plugin-req-ref-coveralls)

<!---2--></details>

<!---2--><details>
<!---2--><summary>Variables</summary>

- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---2--></details>

##### >>>> badges/circleci

_Updating `README.md` using `merge-below-title`._

- Display [circleci](https://circleci.com/) badge in README.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ README.md
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [circleci](#blackfluxrobo-config-plugin-req-ref-circleci)

<!---2--></details>

<!---2--><details>
<!---2--><summary>Variables</summary>

- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---2--></details>

------

<!---1--></details>

#### >>> `dependabot/@default-js`

Recommended base [dependabot configuration](https://dependabot.com/) for javascript projects.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .dependabot
   └─ config.yml
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)
- [github](#blackfluxrobo-config-plugin-req-ref-github)
- [javascript](#blackfluxrobo-config-plugin-req-ref-javascript)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Details</summary>

##### >>>> dependabot/js-instant

_Updating `.dependabot/config.yml` using `overwrite`._

- Configure dependabot to instantly merge javascript dependency updates into the `dev` branch.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ .dependabot
   └─ config.yml
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)
- [github](#blackfluxrobo-config-plugin-req-ref-github)
- [javascript](#blackfluxrobo-config-plugin-req-ref-javascript)

<!---2--></details>

------

<!---1--></details>

#### >>> `git/@default`

Recommended base configuration when using [git](https://en.wikipedia.org/wiki/Git).

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .gitignore
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [git](#blackfluxrobo-config-plugin-req-ref-git)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Details</summary>

##### >>>> git/gitignore

_Updating `.gitignore` using `unique-top`._

- Inject recommended entries into [gitignore file](https://help.github.com/en/articles/ignoring-files).
- Default ignores for JetBrains IDE.
- Default ignores for OSX
- Default ignores for NodeJs

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ .gitignore
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [git](#blackfluxrobo-config-plugin-req-ref-git)

<!---2--></details>

------

<!---1--></details>

#### >>> `license/@MIT-npm`

Recommended base configuration when using MIT License with npm.

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
├─ LICENSE
└─ package.json
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [npm](#blackfluxrobo-config-plugin-req-ref-npm)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [ownerName](#blackfluxrobo-config-plugin-var-ref-ownername)
- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Details</summary>

##### >>>> license/MIT-LICENSE

_Updating `LICENSE` using `overwrite`._

- Generate [MIT license](https://en.wikipedia.org/wiki/MIT_License) file.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ LICENSE
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Variables</summary>

- [ownerName](#blackfluxrobo-config-plugin-var-ref-ownername)

<!---2--></details>

##### >>>> license/MIT-npm

_Updating `package.json` using `merge-shallow`._

- Link MIT license file into [npm](https://www.npmjs.com/) configuration.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ package.json
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [npm](#blackfluxrobo-config-plugin-req-ref-npm)

<!---2--></details>

<!---2--><details>
<!---2--><summary>Variables</summary>

- [ownerName](#blackfluxrobo-config-plugin-var-ref-ownername)
- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---2--></details>

------

<!---1--></details>

#### >>> `npm/@default`

Recommended base configuration when using [npm](https://www.npmjs.com/).

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .npmignore
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [npm](#blackfluxrobo-config-plugin-req-ref-npm)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Details</summary>

##### >>>> npm/npmignore

_Updating `.npmignore` using `unique-top`._

- Inject comment into .npmignore explaining when to use it.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ .npmignore
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [npm](#blackfluxrobo-config-plugin-req-ref-npm)

<!---2--></details>

------

<!---1--></details>

#### >>> `semantic-release/@default`

Recommended base configuration when using [semantic-release](https://github.com/semantic-release/semantic-release).

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .releaserc.json
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Details</summary>

##### >>>> semantic-release/commit-conventions

_Updating `.releaserc.json` using `overwrite`._

- Slightly extended [release commit convention](https://github.com/semantic-release/semantic-release#commit-message-format) for semantic-release.

<!---2--><details>
<!---2--><summary>Targets</summary>

```
project
└─ .releaserc.json
```

<!---2--></details>

<!---2--><details>
<!---2--><summary>Requires</summary>

- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)

<!---2--></details>

------

<!---1--></details>

#### >>> circleci/npm-opensource:two-branch

_Updating `.circleci/config.yml` using `overwrite`._

- Restrictive two-branch [gally](https://github.com/loopmediagroup/gally#readme) config. Custom for npm open source packages.
- TODO

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .circleci
   └─ config.yml
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [npm](#blackfluxrobo-config-plugin-req-ref-npm)
- [yarn](#blackfluxrobo-config-plugin-req-ref-yarn)
- [gally](#blackfluxrobo-config-plugin-req-ref-gally)
- [github](#blackfluxrobo-config-plugin-req-ref-github)
- [circleci](#blackfluxrobo-config-plugin-req-ref-circleci)
- [coveralls](#blackfluxrobo-config-plugin-req-ref-coveralls)
- [dependabot](#blackfluxrobo-config-plugin-req-ref-dependabot)
- [semantic-release](#blackfluxrobo-config-plugin-req-ref-semantic-release)

<!---1--></details>

#### >>> gally/npm-opensource:two-branch

_Updating `.gally.json` using `overwrite`._

- Restrictive two-branch [gally](https://github.com/loopmediagroup/gally#readme) config. Custom for npm open source packages.
- TODO ...

<!---1--><details>
<!---1--><summary>Targets</summary>

```
project
└─ .gally.json
```

<!---1--></details>

<!---1--><details>
<!---1--><summary>Requires</summary>

- [circleci](#blackfluxrobo-config-plugin-req-ref-circleci)
- [gally](#blackfluxrobo-config-plugin-req-ref-gally)
- [github](#blackfluxrobo-config-plugin-req-ref-github)

<!---1--></details>

<!---1--><details>
<!---1--><summary>Variables</summary>

- [owner](#blackfluxrobo-config-plugin-var-ref-owner)
- [mergeBot](#blackfluxrobo-config-plugin-var-ref-mergebot)
- [repoKey](#blackfluxrobo-config-plugin-var-ref-repokey)

<!---1--></details>

</details>

------
------

## Requires

### <a name="blackfluxrobo-config-plugin-req-ref-semantic-release">semantic-release</a>

[Website](https://github.com/semantic-release/semantic-release)

Automates npm package release workflow.

<!---0--><details>
<!---0--><summary>Details</summary>

Automates the package release workflow including:
- determining the next version number
- generating the release notes
- publishing the package

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-npm">npm</a>

[Website](https://docs.npmjs.com/about-npm/)

Javascript package repository.

<!---0--><details>
<!---0--><summary>Details</summary>

Requires the project to be conform with the npm standard, i.e. contain a package.json file.
Does not require the project to be published to npm.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-jetbrains">jetbrains</a>

[Website](https://www.jetbrains.com)

Collection of various IDEs.

<!---0--><details>
<!---0--><summary>Details</summary>

Collection of various IDEs. There exists one for every major programming language and 
they are all very similar (i.e. shortcuts, layout), which makes them great when switching languages.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-nyc">nyc</a>

[Website](https://github.com/istanbuljs/nyc#readme)

Coverage testing for javascript projects.

<!---0--><details>
<!---0--><summary>Details</summary>

A major coverage testing framework for javascript.
Comes with all the bells and whistles.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-git">git</a>

[Website](https://git-scm.com/)

Version control system.

<!---0--><details>
<!---0--><summary>Details</summary>

The most used version control system. Not to be confused with github (which uses git).

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-dependabot">dependabot</a>

[Website](https://dependabot.com/)

Automatic dependency updates.

<!---0--><details>
<!---0--><summary>Details</summary>

Makes dependency updates very easy by automatically creating pull requests in your repo.
All major programming languages are supported or work is done towards supporting them.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-github">github</a>

[Website](https://github.com/)

Major development platform powered by git.

<!---0--><details>
<!---0--><summary>Details</summary>

GitHub is a code hosting platform for collaboration and version control.
Lets you and others work together on projects.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-javascript">javascript</a>

[Website](https://en.wikipedia.org/wiki/JavaScript)

Programming Language.

<!---0--><details>
<!---0--><summary>Details</summary>

JavaScript, often abbreviated as JS, is a high-level, interpreted programming language that conforms to the ECMAScript specification.
It is characterized as dynamic, weakly typed, prototype-based and multi-paradigm.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-js-gardener">js-gardener</a>

[Website](https://github.com/blackflux/js-gardener#readme)

NodeJs Project Management.

<!---0--><details>
<!---0--><summary>Details</summary>

Enforces and helps setting up best practices around NodeJs projects.
Enforces highest code quality and minimizes package setup and maintenance complexity - so you can focus on writing code.
Highly recommended if you are getting started with a new package and extremely useful if you are maintaining multiple packages.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-npm-published">npm-published</a>

[Website](https://docs.npmjs.com/about-npm/)

Javascript package repository published.

<!---0--><details>
<!---0--><summary>Details</summary>

Requires the project to be published to npm either as a private or public package.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-david-dm">david-dm</a>

[Website](https://david-dm.org/)

Dependency badge for javascript github repositories.

<!---0--><details>
<!---0--><summary>Details</summary>

Enables displaying of a status badge indicated whether the dependencies are outdated.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-coveralls">coveralls</a>

[Website](https://coveralls.io/)

Showcase and analyze coverage reports.

<!---0--><details>
<!---0--><summary>Details</summary>

Enables displaying of a status badge indicated code coverage percent of the project.
Furthermore allows anyone to easily drill down into missing coverage or coverage changes.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-circleci">circleci</a>

[Website](https://circleci.com/)

Run automated jobs using docker containers.

<!---0--><details>
<!---0--><summary>Details</summary>

Allows set up for ci/cd using docker containers.
Automates development process quickly, safely, and at scale.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-yarn">yarn</a>

[Website](https://yarnpkg.com/)

Dependency management similar to npm.

<!---0--><details>
<!---0--><summary>Details</summary>

Very similar functionality to npm cli. However there are some significant differences.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-req-ref-gally">gally</a>

[Website](https://github.com/loopmediagroup/gally)

Automation around github.com Repository Management

<!---0--><details>
<!---0--><summary>Details</summary>

Allows management of github.com repositories through configuration.
Very powerful when you need to synchronize settings across multiple repositories.

<!---0--></details>

------
------

## Variables

### <a name="blackfluxrobo-config-plugin-var-ref-ownername">ownerName</a>

Type: `string`

Name of the owner of this project.

<!---0--><details>
<!---0--><summary>Details</summary>

The owner name of the project is the name of the person or organization publishing the project under their license.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-var-ref-repokey">repoKey</a>

Type: `string`

Repository key.

<!---0--><details>
<!---0--><summary>Details</summary>

The repository key contains the owner or organization of the project and the repository name itself, separated by a slash.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-var-ref-projectname">projectName</a>

Type: `string`

Name of the project.

<!---0--><details>
<!---0--><summary>Details</summary>

The project name is in most cases identical to the repository name.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-var-ref-packagename">packageName</a>

Type: `string`

Name of the package on npm.

<!---0--><details>
<!---0--><summary>Details</summary>

The name of the project as published to npm.
Note that for scoped packages the name can differ significantly from the repo name.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-var-ref-owner">owner</a>

Type: `string`

The owner of the code on github.

<!---0--><details>
<!---0--><summary>Details</summary>

The code owner is the gatekeeper of the project, ultimately responsible for all changes.

<!---0--></details>

### <a name="blackfluxrobo-config-plugin-var-ref-mergebot">mergeBot</a>

Type: `string`

The github name of the bot used for automatic merging.

<!---0--><details>
<!---0--><summary>Details</summary>


<!---0--></details>
