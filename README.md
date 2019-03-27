
# Dev Notebook

My curated list of dev hacks, notes and fixes.
Props to [@xemasiv](https://github.com/xemasiv) for the [idea](https://github.com/xemasiv/my-dev-fixes))

* [Change port for create-react-app](#change-port-for-create-react-app)
* [Close single simulator in Xcode](#close-single-simulator-in-xcode)
* [React Native Expo changes not reloaded](#react-native-expo-changes-not-reloaded)
* [Safe CSS Defaults](#safe-css-defaults)
* [Online Code Editor](#online-code-editor)
* [Hot Links](#hot-links)
* [Per-repository SSH keys](#per-repository-ssh-keys)
* [Kill Chrome Command](#kill-chrome-command)
* [Lofty Concepts](#lofty-concepts)
* [Cheat Sheets](#cheat-sheets)
* [Axios catch error](#axios-catch-error)
* [Concepts](#concepts)
	* [Redux](#redux)


## Change port for create-react-app
Change the start script to from 
```
"start": "react-scripts start"
```
to
```
"start": "PORT=3006 react-scripts start"
```
[Source](https://stackoverflow.com/questions/40714583/how-to-specify-a-port-to-run-a-create-react-app-based-project)

## Close single simulator in Xcode

Select Simulator.. Go into File Menu -> Close window or press [Command + W ]. It will close the simulator which is on top.
[Source](https://stackoverflow.com/questions/45165635/how-to-quit-or-close-single-simulator-from-opened-multiple-simulator-in-xcode-9)

## React Native expo changes not reloaded

```
rm .git/index.lock
```
[Source](https://github.com/facebook/react-native/issues/4357#issuecomment-394448806)

## Safe CSS Defaults

| Property          | Value                                                                                        | 
|-------------------|----------------------------------------------------------------------------------------------| 
| background        | "transparent (transparent stands for rgba(0, 0, 0, 0)) or none or 0 0"                       | 
| border            | `none` or `0`                                                                                | 
| border-image      | `none`                                                                                       | 
| border-radius     | `0`                                                                                          | 
| box-shadow        | `none`                                                                                       | 
| clear             | `none`                                                                                       | 
| color             | "No value, so best option is to use inherit to cascade from a parent element’s color value." | 
| content           | `normal`                                                                                     | 
| display           | `inline`                                                                                       | 
| float             | `none`                                                                                         | 
| font              | `normal`                                                                                       | 
| height            | `auto`                                                                                         | 
| letter-spacing    | `normal`                                                                                       | 
| line-height       | `normal`                                                                                       | 
| max-width         | `none`                                                                                         | 
| max-height        | `none`                                                                                         | 
| min-width         | `0`                                                                                            | 
| min-height        | `0`                                                                                            | 
| opacity           | `1`                                                                                            | 
| overflow          | `visible`                                                                                      | 
| page-break-inside | `auto`                                                                                         | 
| position          | `static` (not relative)                                                                        | 
| text-shadow       | `none`                                                                                         | 
| text-transform    | `none`                                                                                         | 
| transform         | `none`                                                                                         | 
| transition        | `none`                                                                                         | 
| vertical-align    | `baseline`                                                                                     | 
| visibility        | `visible`                                                                                      | 
| white-space       | `normal`                                                                                       | 
| width             | `auto`                                                                                         | 
| word-spacing      | `normal`                                                                                       | 
| z-index           | `auto` (not none or 0)                                                                         | 

[Source](http://nimbupani.com/safe-css-defaults.html)

## Hot Links
* [devhints](https://devhints.io/)
* [python-vs-javascript](https://sayazamurai.github.io/python-vs-javascript/)

## Per-repository SSH keys
If you want to use different keys depending on the repository you are working on, you can issue the following command while inside your repository:

```
git config core.sshCommand "ssh -o IdentitiesOnly=yes -i ~/.ssh/private-key-filename-for-this-repository -F /dev/null"
```

This will not use the SSH Agent and requires at least Git 2.10.

[Source](https://docs.gitlab.com/ee/ssh/#per-repository-ssh-keys)


## Kill Chrome Command
```
killall -9 "Google Chrome"
```

## Lofty Concepts
* [Lerna and Yarn Workspaces](https://medium.com/@NareshBhatia/sharing-ui-components-with-lerna-and-yarn-workspaces-be1ebca06efe)


## Code Playgrounds
* front-end languages like HTML, CSS, JavaScript etc [Codepen](https://codepen.io/)
* Better for web apps with support for imports etc [codesandbox](https://codesandbox.io/)
* Like codepen with support for serverside (Node, PHP etc) [Glitch](https://glitch.com/edit/#!/clever-albacore)
* React Native Flexbox [Yoga Layout](https://yogalayout.com/playground)
* Dexter's Lab (The playground of lodash and lodash/fp) [Dexter's Lab](http://dexters-lab.io/)
* Like Codepen but for React Native [Snack](https://snack.expo.io)

## Cheat Sheets
* [The Full React Native Layout Cheat Sheet](https://medium.com/@drorbiran/the-full-react-native-layout-cheat-sheet-a4147802405c/)


## Axios catch error
* [Axios catch error returns javascript error not server response](https://github.com/axios/axios/issues/960#issuecomment-398269712/)

## Disable eslint for a file
```
/* eslint-disable */
```

## Concepts

### Redux
* [beginners guide to redux middleware](https://www.codementor.io/vkarpov/beginner-s-guide-to-redux-middleware-du107uyud)

