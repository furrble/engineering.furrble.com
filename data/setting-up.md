# Git Setup

git is a version control system we will be using. Now, all the usual tutorials will be useful if you know git.
Otherwise, contributing code can be tough in controlled environments.

Here are a few rules:
1. All the code is written to `dev` branch of any project. It is later merged to master to prevent bad code in production.
2. All commit messages must clearly describe whatever you are willing to do.
3. All contributions must be made on a Pull Request, which in turn be reviewed by at-least 1 other developer.

This can be difficult. So let's see how can one get started with the process.

## Commit Signing

Please make sure that your local git client is configured properly:
```
$ git config --global user.name "John Doe"

$ git config --global user.email john@furrytails.in
```
Please ensure that the email `john@furrytails.in` is there in your GitHub Account. If you want help with that,
please [see this guide by GitHub](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/adding-an-email-address-to-your-github-account)

This will ensure every commit you make is properly signed.

## Git Clone

Now, you are all set and prepared to contribute, so here we start. We will keep placeholders in all the commands,
all you have to do is fill them with the name of the respective repository.

First of all, **fork** the repository in your personal GitHub namespace. If you want to know how to do that, have a look at this
[guide by GitHub](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo).

Let's assume, you wanted to fork [FurryTails/learn](https://github.com/FurryTailsIN/learn). You will now have a repository in **[Your-User-Name]/learn**.

```
$ git clone https://github.com/[Your-User-Name]/learn.git

$ cd learn/

$ git remote add upstream https://github.com/FurryTailsIN/learn.git

$ git checkout dev

```
