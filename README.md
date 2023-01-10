# This is the demo project to show how submodule works with Next.js

Reference: [Git Submodules basic explanation](https://gist.github.com/gitaarik/8735255)

Submodule repo: https://github.com/TOMO-YOSHI/components

## Commands
- Make clone

  `git clone https://github.com/TOMO-YOSHI/components-submodule-demo-website.git`

- Go into the project

  `cd components-submodule-demo-website`

- Install dependencies

  `yarn install`

- Go into the submodule

  `cd ./src/components`

- Get the information about the submodule

  `git submodule init`

- Update the code of your submodules

  `git submodule update`

- Go back to the root

  `cd ../..`

- Run Next.js dev server

  `yarn dev`

## How I set up the second project

- Made project by `yarn create next-app` command

- Created `src` dir and moved `pages` and `styles` dir.

- Created `components` dir in `src`

- `cd src`

- Added submodule to the project `git submodule add https://github.com/TOMO-YOSHI/components.git ./components`

## How to commit the submodule
Submodules are not tracked by the git commands at the root dir. Therefore, devs have to run `git add`, `git commit`, and `git push` separately.

## How to pull and update the submodule after the remote repo has been updated

- `cd ./src/components/`

- `git pull`

- ~~`git pull --recurse-submodules`~~

- ~~`git submodule update --remote` ~~