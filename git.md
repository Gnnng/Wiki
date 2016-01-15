Git
=====


## Commands

- 提交文件中的部分代码: `git add -p [filename]`
- 更改最后一次的 commit message: `git commit --amend`
- 修改之前的提交历史: `git rebase -i [SHA-1]`
- 按指定 date 提交 commit: `git commit --date="Thu Jan 14 20:41:34 2015 +0800"`

## Commit Message Formatting

> This formatting comes from "Angular JS Git Commit Message Conventions" 
> ([link](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/edit#))
>
> PS: 对于纯博客的内容，直接使用 `docs`

Pattern:

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

### Message Header

A single line contains a `<type>` description, an optional `<scope>` and a `<subject>`

#### `<type>`

- **feat**: feature
- **fix**: bug fix
- **docs**: documentation
- **style**: formatting, missing semi colons, ...
- **refactor**: not bug involved
- **test**: when adding new test suite
- **chore**: maintain

#### `<scope>`

Scope can be anything specifying place of the commit change.

#### `<subject>`

A very short description of the change:

- use imperative, present tense: "change" not "changed" nor "changes"
- don't capitalize first letter
- no dot (.) at the end

### Message Body

- use imperative, present tense: "change" not "changed" nor "changes"
- includes motivation for the change and contrasts with previous behavior

### Message Footer

#### Breaking Changes

All breaking changes have to be mentioned as a breaking change block in the folder,
which should start with the word BREAKING CHANGE: with a space or two newlines. The rest
of the commit message is then the description of the change, justification and migration
notes.

#### Referencing issues

Closed bugs should be listed on a separate line in the footer prefixed with "Closes" keyword like this:

```
Closes #234
```

or in case of multiple issues:

```
Closes #234, #345, #456
```


## Git Branching Model

Vincent Driessen's branching model.

see more on [here](http://nvie.com/posts/a-successful-git-branching-model/) and use [git-flow](https://github.com/nvie/gitflow)


![](http://nvie.com/img/git-model@2x.png)




