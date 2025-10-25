# Documentation Hub Website

This is the main website for the Sessie Research Group. More information regarding our site can be found [here](https://sessieresearchatsau.github.io/). As per the [GitHub Pages docs on URLs](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#types-of-github-pages-sites), the name of this repository is as it is due to being the main organization website.

The [Docsify](https://docsify.js.org/) tool was used to develop this website. It allows us to create nice documentation sites very quickly using mostly just [markdown]([Markdown](https://sessieresearchatsau.github.io/#/software/markdown)). To create a similar repository-specific documentation site, either follow the instructions on Docsify's documentation or simply copy the contents of this repository and modify the markdown files to your liking (but don't forget to update the index.html for your website).

We also use the following plugins to enable additional features/custimizations:
- <https://jhildenbiddle.github.io/docsify-themeable/#/>
- <https://docsify.js.org/#/plugins?id=full-text-search>
- <https://docsify.js.org/#/plugins?id=copy-to-clipboard>
- <https://scruel.github.io/docsify-latex>
- <https://github.com/Leward/mermaid-docsify>

## Editing the documentation

Editing the documentation is very easy. If you have the markdown files cloned on to your computer, simply open a file in any editor (VS Code or Obsidian are nice), make a change, and push the change. Alternately, you can [make edits right here in GitHub]([Editing files - GitHub Docs](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files))!

It should, however, be noted that if you want to see your changes rendered on the website right away, you must download Docsify so that you can serve it locally over `localhost`. This way changes are reflected immediately in your browser window. After you are happy with your changes, you then can push them to GitHub. The instructions for setting up Docsify locally are covered below.

## Setting up Docsify for a better editing experience

To set up Docsify locally, npm (Node Package Manager) must be installed. The easiest way to do this is using an nvm (Node Version Manager). For windows, [nvm-windows](https://github.com/coreybutler/nvm-windows)works well. Install it by clicking on the [nvm-setup.exe](https://github.com/coreybutler/nvm-windows/releases/download/1.2.2/nvm-setup.exe) on the Releases page. After installing the nvm, download npm by running `nvm install latest` in the terminal. This will install npm. For other platforms, simply follow these docs: [Downloading and installing Node.js and npm | npm Docs](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm).

Now that npm is installed, install Docsify by running `npm i docsify-cli -g` in the terminal.

You are now good to go! Simply `cd` to the directory where the markdown site is, run the `docsify serve` command, and navigate to the `http://localhost:3000` URL (or whichever URL Docsify provides) in your browser. Here, any changes to the markdown files will immediately be rendered!

Please follow the official Docsify docs for more details on changing the sidebar, theme, etc.

## Publishing with GitHub Pages
Please read [What is GitHub Pages? - GitHub Docs](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages) for more details on using GitHub Pages.

For repository-specific documentation, please place all markdown (other than the README.md which is the main documentation for the repo) in a subdirectory called `./docs`. This where your site should reside. Even if you don't use a site with GitHub Pages, documentation for any repository/project should still be placed in such a subdirectory.

You can then use GitHub pages by: `Repository Settings > Pages > Branch Dropdown [Select from master branch] & [select "/docs" as the directory from which to serve the site]`. Really, you must serve the site from wherever the `index.html` resides; so if it is in the root directory, simply select `/root` rather than `/docs`. Of course, you may also unpublish the site by clicking `Unpublish site` at any time.

Once you have GitHub pages setup and running for a repository, any changes to the markdown will be automatically be deployed (although it could take a few seconds to a minute; this is why a local install of Docsify is helpful for quick feedback).
