# Dev Notebook

My curated list of dev hacks, notes and fixes.
Props to [@xemasiv](https://github.com/xemasiv) for the [idea](https://github.com/xemasiv/my-dev-fixes))

* [Change port for create-react-app](#change-port-for-create-react-app)
* [Close single simulator in Xcode](#close-single-simulator-in-xcode)
* [React Native Expo changes not reloaded](#react-native-expo-changes-not-reloaded)
* [Hot Links](#hot-links)

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

## Hot Links
* [devhints/](https://devhints.io/)
