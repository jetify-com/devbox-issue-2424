This PR demonstrates using a local plugin that can be included in `devbox.json`
to avoid needing to re-declare packages in multiple devbox.jsons

```
% devbox shell
Info: Ensuring packages are installed.
Info: Installing the following packages to the nix store: bat@0.24.0, just@1.30.1, jq@1.7.1
✓ Computed the Devbox environment.
Starting a devbox shell...

(devbox) issue-2424 % command -v bat
/Users/savil/code/jetpack/devbox-projects/issue-2424/.devbox/nix/profile/default/bin/bat

(devbox) issue-2424 % command -v just
/Users/savil/code/jetpack/devbox-projects/issue-2424/.devbox/nix/profile/default/bin/just

(devbox) issue-2424 % command -v jq
/Users/savil/code/jetpack/devbox-projects/issue-2424/.devbox/nix/profile/default/bin/jq
```
