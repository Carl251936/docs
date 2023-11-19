---
title: About GitHub Desktop
shortTitle: 'About'
intro: '{% data variables.product.prodname_desktop %} helps you work with projects hosted on {% data variables.product.prodname_dotcom %}.'
versions:
  feature: desktop
redirect_from:
  - /desktop/installing-and-configuring-github-desktop/overview/about-github-desktop
  - /github/getting-started-with-github/github-desktop
  - /github/getting-started-with-github/using-github/github-desktop
  - /get-started/using-github/github-desktop
---

## About {% data variables.product.prodname_desktop %}

{% data variables.product.prodname_desktop %} is a free, open source application that helps you to work with files hosted on {% data variables.product.prodname_dotcom %} or other Git hosting services.

You can use {% data variables.product.prodname_desktop %} alongside any tools you need to contribute to a project. For example, a typical workflow would be to use {% data variables.product.prodname_desktop %} to download a {% data variables.product.prodname_dotcom %} repository to your computer and create a new branch, use an editor such as {% data variables.product.prodname_vscode %} to make changes to the code, then return to {% data variables.product.prodname_desktop %} to commit and push the changes to {% data variables.product.prodname_dotcom %}.

## About the benefits of {% data variables.product.prodname_desktop %}

Like any tool for contributing changes to repositories on {% data variables.product.prodname_dotcom %}, {% data variables.product.prodname_desktop %} is built around the version control software Git. If you're new to Git and {% data variables.product.prodname_dotcom %}, you may find it easier to get started with {% data variables.product.prodname_desktop %} than you would using Git on the command line. Because {% data variables.product.prodname_desktop %} has a graphical user interface, it simplifies many of the aspects of Git that can be challenging for new users, such as memorizing commands and visualizing the changes you're making.

Even if you have experience with command-line Git, you may benefit from incorporating {% data variables.product.prodname_desktop %} into your work. If you frequently need to look up syntax for less common Git commands, such as choosing which changed lines to include in a commit or adding a co-author to a commit, you may benefit from switching to {% data variables.product.prodname_desktop %} to perform these commands.

Because {% data variables.product.prodname_desktop %} makes commands like these easy to find, and helps you visualize the changes you're introducing with an integrated diff view, it encourages best practices and helps you to create an accurate and easy-to-follow commit history so other collaborators on a project can easily review your work.

Unlike other Git clients, {% data variables.product.prodname_desktop %} is specifically designed for use with {% data variables.product.prodname_dotcom %}, so it can make you more productive when working with repositories on {% data variables.product.prodname_dotcom %}. For example, you can authenticate to {% data variables.product.prodname_dotcom_the_website %} or {% data variables.product.prodname_ghe_server %} quickly, without needing to use a separate credential manager, and you can check out a pull request to run checks without needing to open your browser.

## Getting started

{% data variables.product.prodname_desktop %} is available for Windows and macOS. For information about installing and getting started with {% data variables.product.prodname_desktop %}, see "[AUTOTITLE](/desktop/overview/getting-started-with-github-desktop)."

If you're interested in the open source {% data variables.product.prodname_desktop %} project, you can see the roadmap, contribute to the project, or open an issue to provide feedback in the [`desktop/desktop`](https://github.com/desktop/desktop) repository.

## Further reading

- "[AUTOTITLE](/get-started/using-git/about-git)"
REMIX DEFAULT WORKSPACE

Remix default workspace is present when:
i. Remix loads for the very first time 
ii. A new workspace is created with 'Default' template
iii. There are no files existing in the File Explorer

This workspace contains 3 directories:

1. 'contracts': Holds three contracts with increasing levels of complexity.
2. 'scripts': Contains four typescript files to deploy a contract. It is explained below.
3. 'tests': Contains one Solidity test file for 'Ballot' contract & one JS test file for 'Storage' contract.

SCRIPTS

The 'scripts' folder has four typescript files which help to deploy the 'Storage' contract using 'web3.js' and 'ethers.js' libraries.

For the deployment of any other contract, just update the contract's name from 'Storage' to the desired contract and provide constructor arguments accordingly 
in the file `deploy_with_ethers.ts` or  `deploy_with_web3.ts`

In the 'tests' folder there is a script containing Mocha-Chai unit tests for 'Storage' contract.

To run a script, right click on file name in the file explorer and click 'Run'. Remember, Solidity file must already be compiled.
Output from script will appear in remix terminal.

Please note, require/import is supported in a limited manner for Remix supported modules.
For now, modules supported by Remix are ethers, web3, swarmgw, chai, multihashes, remix and hardhat only for hardhat.ethers object/plugin.
For unsupported modules, an error like this will be thrown: '<module_name> module require is not supported by Remix IDE' will be shown.
