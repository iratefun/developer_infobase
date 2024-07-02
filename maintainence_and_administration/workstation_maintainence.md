# Workstation Maintainence

To make maintainence tasks simpler, the following bash script is utilized.  This script will utilize abraxas (tool) to build all projects that have associated builders, ensure the builds were successful, and then log the results of the manufacturing of those packages.  Then all git_controlled repositories will have their files added, committed, and pushed to the remote repos.  This is not an issue considering these are my repos only, and I don't have to worry about conflicts.

```
#!/bin/bash
# Workstation Maintainence Script

# invoke abraxas package manufacturer (builds packages)
pushd ./
cd /home/tourist/workspace/software/git_controlled/prcr__abraxas__runnable/
node ./prcr__abraxas__runnable.js --config_file "/home/tourist/workspace/configs/manufacturer/prcr__manufacturer_config.json"
popd

# invoke sisyphus task runner (runs admin/maintainence tasks)
pushd ./
cd /home/tourist/workspace/software/git_controlled/prcr__sisyphus__runnable/
node ./prcr__sisyphus__runnable.js --config_file "/home/tourist/workspace/configs/sisyphus/build_all_git_add_all_git_commit_all_git_push_all.sisyphus.js"
popd

```
