# fluxboard-styles

Shared styles and variables for front end and back end Fluxboard apps.

To load the latest styles from the master branch of this repo in an application, run
`rm -rf node_modules/mapdwell-base-styles && npm install`
in that application's directory.

Watchman can be used to access load local, in-development files into an application. In this repo's directory, run the following to watch for changes and copy files directly into node_modules of other repos.

- `watchman -- trigger $PWD cr '**/*.scss' -- sh cp_to_mapdwell.sh `
- `watchman -- trigger $PWD cr '**/*.scss' -- sh cp_to_fluxboard.sh `

Keep in mind this solution assumes `mapdwell-base-styles` is in the same local directory as the `mapdwell` and `fluxboard` repos. Use `watchman watch-del-all` to manually remove these commands.

,,,
