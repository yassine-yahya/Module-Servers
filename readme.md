# Welcome to Node

All the coursework is listed as issues on this repo. You will copy these issues to your Coursework Planner, which is one repo that will hold all your coursework and assignments for the entire course.

If you do not already have your own Coursework Planner, set one up now:

https://github.com/CodeYourFuture/Coursework-Planner

## Troubleshooting

### Version management with `nvm`

At some point you will begin to hit repos that expect a specific version of Node. This repo expects you to use Node version [20.4.0](https://nodejs.org/en/blog/release/v20.4.0) or higher.

But other repos may expect an older version. Mentors will likely suggest you use [Node Version Manager](https://www.freecodecamp.org/news/node-version-manager-nvm-install-guide/), which is correct. This is how professional developers handle this common problem.

You can use `nvm` to manage your Node versions when this comes up.

### Workspaces

However, if you do now have NVM installed: _this repo uses workspaces_. If you try to switch Node versions _inside_ the subdirs, then, you will get errors like

```zsh
npm ERR! code ENOWORKSPACES
npm ERR! This command does not support workspaces.
```

And you may fall down a rabbit hole of nvm prefix management. This is not a good use of your time. Use the Node version specified in the `.nvmrc` file and set it while you are in the root of this folder. Do this by typing:

```zsh
nvm use
```

In the root of this folder. This will set the correct version of Node for you, if you have NVM installed.
