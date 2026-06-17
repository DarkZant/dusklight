## Instructions to update this branch to the latest release
1. Sync the main branch of the fork with the Dusklight repository.
1. Checkout to the main branch with `Git > Manage Branches` or `git checkout main`.
2. Pull the sync changes from the fork into the local main branch.
3. *Optional*: If the most recent commit of the main branch of Dusklight is more recent than the desired release, do `git reset --hard v1.2.3` (change version tag as needed). This sets your branch to the desired release.
4. Do `git submodule update --init --recursive` to update **aurora** and other libraries.
1. Do `git fetch upstream --tags` to obtain the tags of the latest versions.
1. Checkout to the playing branch with `Git > Manage Branches` or `git checkout playing`.
5. Merge the **main** branch into the **playing** branch with `Git > Manage Branches > Right Click main > Merge 'main' into 'playing'`.
6. Do `Project > Delete Cache and Reconfigure` to reset CMake.
7. If not already done, select `Windows (MSVC)` and `dusklight.exe` as run configurations.
8. Click the `dusklight.exe` filled green arrow to build and compile the code. This should also launch the game.
9. Close the game and click the hollow green arrow to run the game without debugging.
10. Enjoy the game! 