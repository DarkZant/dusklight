## Instructions to update this branch to the latest release
1. Sync the main branch of the [fork on GitHub](https://github.com/DarkZant/dusklight) with the [Dusklight repository](https://github.com/TwilitRealm/dusklight).
1. Checkout to the main branch with `Git > Manage Branches` or `git checkout main`.
1. If not already done, add the Dusklight repository as an upstream remote with `git remote add upstream https://github.com/TwilitRealm/dusklight`.
1. Pull the synced changes from the fork into the local main branch.
1. Do `git fetch upstream --tags` to obtain the tags of the latest versions. This step is crucial to have **DarkZant Edition** show up.
1. *Optional*: If the most recent commit of the main branch of Dusklight is more recent than the desired release, do `git reset --hard v1.2.3` (change version tag as needed). This sets the local main branch to the desired release.
1. Do `git submodule update --init --recursive` to update **aurora** and other libraries.
1. Checkout to the playing branch with `Git > Manage Branches` or `git checkout playing`.
1. Merge the **main** branch into the **playing** branch with `Git > Manage Branches > Right Click 'main' > Merge 'main' into 'playing'`.
1. Do `Project > Delete Cache and Reconfigure` to reset CMake.
1. If not already done, select `Windows (MSVC)` and `dusklight.exe` as run configurations.
1. Click the `Start Without Debugging` hollow green arrow to build and compile the code. This should also launch the game.
1. Create a shorcut of the game on the Desktop. The executable is at `dusklight/build/windows-msvc/dusklight.exe`.
1. Enjoy **Dusklight: DarkZant Edition**! 