react-router! What an amazing build process!

`npm run build` builds into the `build/` directory. This is what actually gets published to npm.
There is no easy way to ask npm to install just this subdirectory of a github repository.

Solution:

  1. `cd build`
  1. `git init`
  1. `git branch -m [your_build_branch_name]`
  1. `git add *`
  1. `git commit` (write a commit message)
  1. `git remote add origin https://github.com/captain401/react-router.git`
  1. `git push origin [your_build_branch_name]`
  1. Add npm dependency on `captain401.com/react-router#[your_build_branch_name]`
