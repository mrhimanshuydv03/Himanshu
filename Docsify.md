![](https://lh7-us.googleusercontent.com/D_eaC78Ov4siaZ5NjspxI4eyL95cBd0zuM9kX1-ZUzRq6Irx2Br0JxYLJUJ-ZGKs4cYqEvoVGq-pSdMfsVSAH0nQ_GoVpomQVw8V2b8_7ExOMXRiHvs0hKYGWuofAooH_HOO1Epdut31Gy34jVxN4I5XbCWCRneArXBDCthWZZ83xH_dlw6wjg83qx1s1w)                                                                                                           By:-Himanshu

# TABLE OF CONTENT 

[1.What is Docsify ? ](#1what-is-docsify-)

[2.Why Docsify ?](#2why-docsify-)

[3. Features of docsify](#3-features-of-docsify--)

[4. Advantage and Disadvantage of Docsify ](#4-advantage-and-Disadvantage-of-docsify-)

[5. Step by step guide to installation and Setup](#5-step-by-step-guide-to-installation-and-setup)


# 1.What is Docsify ?

- Docsify is a simple and lightweight documentation generator. You can start using it without having any knowledge of JavaScript or React. Docsify comes with zero configuration, no statically built HTML files, multiple theme support, inbuilt plugin API, and full-text search support with a plugin.

* Docsify is a documentation site generator that allows you to create beautiful, searchable documentation websites using markdown files. It's often used by developers and teams to create documentation for their projects in a simple and efficient way.


# 2.Why Docsify ?

- Docsify generates our documentation website on the fly. Unlike GitBook, it does not generate static html files. Instead, it smartly loads and parses your Markdown files and displays them as a website.

* Versioning: Docsify supports versioning, making it easier to manage different versions of your documentation for various releases or updates.

- Active Community: Docsify has an active and growing community of users. This means you can find support, documentation, and plugins/extensions created by the community to enhance the functionality of Docsify.

* Free and Open Source: Docsify is an open-source project, meaning it's free to use and you can contribute to its development or customize it based on your requirements.

* Overall, Docsify is a lightweight and user-friendly documentation solution suitable for projects of varying sizes. It provides a quick and efficient way to create, organize, and present documentation for your software projects.


# 3. Features of docsify -

- ## No statically built html files

When we say "no statically built HTML files," it means that a website or web application is not generating HTML files in advance. In a static website, HTML files are pre-built and stored, and when a user visits a page, they see the pre-rendered content.

- ## Docsify is simple and lightweight 

Docsify is like a simple and lightweight tool for creating and managing documentation websites. It helps you make clean, attractive documentation using easy-to-write files. Instead of building the entire website beforehand, Docsify generates the pages dynamically when someone visits, making it easy to update and manage. It's a straightforward way to showcase information without the hassle of complicated setups.

- ## Smart full-text search plugin

It works like a super-smart index at the back of a book. You type in a word or phrase you're looking for, and Docsify instantly shows you where it appears in your documentation. This makes it easy to find the information you need without manually scanning through every part of your document. It's like having a helpful assistant that quickly points you to the exact spot where your desired words or topics are discussed.

- ## Multiple theme

Docsify's multiple themes allow you to dress up your documentation site in various styles, making it more visually appealing and suitable for different occasions or preferences.

- ## Useful plugin API

In simple terms, a plugin in Docsify is like adding a special feature to your documentation website. It's a bit like getting a cool extra tool that helps you do something specific.

Docsify's plugin API (Application Programming Interface) is like a set of instructions that tells you how to add these special features to your site. It's like a guide that shows you how to use these tools to enhance your documentation.

- ## Emoji support

Emoji support in Docsify is like adding expressive little pictures to your text to make it more fun and engaging. Instead of just using words, you can insert emojis – those small, colorful icons – to convey emotions, reactions, or add a touch of playfulness to your documentation.

- ## Compatible with IE11

When we say "compatible with IE11" in the context of Docsify, it means that Docsify is designed to work smoothly with the Internet Explorer 11 web browser. Internet Explorer 11 (IE11) is an older web browser, and some modern websites or tools may not work well with it. However, Docsify is made in a way that it can be used and viewed properly even if someone is using Internet Explorer 11 to access the documentation. So, people using IE11 won't face any major issues, and they can still read and interact with the documentation as intended.

- ## Support server-side rendering

instead of relying on the user's browser to do all the work to display the content, Docsify can get some assistance from the server. This helps in making sure that the content is ready to be shown when the user asks for it, making the experience faster and more efficient.  


# 4. Advantage and disadvantage of Docsify-

## Advantages of Docsify:

- Easy to Use: Docsify is simple to set up and use, making it beginner-friendly. You don't need to be a coding expert to get started.

* Lightweight: It's not heavy on resources, meaning your documentation site won't be slow to load. This is good for a smooth user experience.

- Dynamic Loading: Docsify loads pages dynamically, which means it only fetches the content when a user requests it. This can make your site faster.

* Markdown Support: Docsify uses Markdown, a simple and readable syntax, making it convenient for content creation.

- Themes and Plugins: There are multiple themes and plugins available, allowing you to customize the look and add extra features without much effort.


## Disadvantages of Docsify:

- Not Ideal for Complex Sites: If you need a complex website with many interactive features, Docsify might not be the best choice. It's more suited for simpler documentation sites.

* Limited Built-in Features: While it's lightweight, Docsify might lack some built-in features compared to more extensive documentation platforms.

- Dependent on JavaScript: Docsify relies on JavaScript, so if a user has it disabled, the site may not function properly for them.

* Less Community and Support: Compared to more mainstream documentation platforms, Docsify may have a smaller community and fewer resources for troubleshooting.

- In summary, Docsify is great for straightforward documentation needs, offering simplicity and speed. However, for more complex websites, you might want to explore other options with broader feature sets.


# 5. Step by step guide to installation and Setup.

Step 1: Install Node.js and npm

- Open a terminal on your Ubuntu system.

* Update the package list to make sure you have the latest 
```
su
```
If you run su without specifying a username, it will prompt you for the root (administrative) password, and upon entering the correct password, you'll switch to the root user account, giving you elevated privileges.
```
sudo apt update
```



sudo: This is a command that stands for "superuser do." It is used to execute commands with elevated or administrative privileges.

apt: Stands for "Advanced Package Tool." It is a package management system used in Ubuntu for installing, updating, and removing software packages.

update, it instructs the package management system to update its information about available software packages.
```
vboxuser@Hunny:~$ su
Password:
root@Hunny:/home/vboxuser# sudo apt update
Hit:1 http://in.archive.ubuntu.com/ubuntu jammy InRelease
Hit:2 http://in.archive.ubuntu.com/ubuntu jammy-updates InRelease
Hit:3 http://security.ubuntu.com/ubuntu jammy-security InRelease
Hit:4 http://in.archive.ubuntu.com/ubur .ubuntu.com/ubuntu jammy-backports InRelease
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
177 packages can be upgraded. Run 'apt list --upgradable' to see them.
root@Hunny:/home/vboxuser# f
```


Step 2: Install Node.js. You can choose to install either the LTS (Long Term Support) version or the latest version. Here, I'll showyou how to install the LTS version:
```
sudo apt install nodejs
```
sudo: This is a command that stands for "superuser do." It's used to execute the following command with administrative privileges.

apt: Stands for "Advanced Package Tool." It's a package management system used in Ubuntu for installing, updating, and removing software packages.

install: This is a specific sub-command of apt. It tells the package manager that you want to install a software package.

nodejs: This is the name of the software package you want to install. In this case, it's Node.js, a JavaScript runtime for executing JavaScript code on the server side.
```
root@Hunny:/home/vboxuser# sudo apt install nodejs
Reading package lists... Done
Building dependency tree. Done
Reading state information... Done
The following additional packages will be installed:
javascript-common libc-ares2 libjs-highlight.js libnode72 nodejs-doc
Suggested packages:
apache2 | lighttpd | httpd npm
The following NEW packages will be installed:
javascript-common libc-ares2 libjs-highlight.js libnode72 nodejs nodejs-doc
0 upgraded, 6 newly installed, o to remove and 177 not upgraded.
Need to get 13.7 MB of archives.
After this operation, 53.9 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://in.archive.ubuntu.com/ubuntu jammy/main amd64 javascript-common all 11+nmu1 [5,936 B]
Get:2 Get:3 http://in.archive.ubuntu.com/ubuntu jammy/universe amd64 libjs-highlight.js all 9.18.5+dfsg1-1 [367 kB] http://in.archive.ubuntu.com/ubuntu jammy-updates/main amd64 libc-ares2 amd64 1.18.1-1ubuntu0.22.04.2 [45.0 kB
Get:4 Get:5 http://in.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 libnode72 amd64 12.22.9~dfsg-1ubuntu3.3 [10.8 http://in.archive.ubuntu.com/ubuntu jammy-updates/unive -updates/universe amd64 nodejs-doc all 12.22.9~dfsg-1ubuntu3.3 [2,410
Get:6 http://in.archive.ubuntu.com/ubuntu jammy-updates/universe amd64 nodejs amd64 12.22.9~dfsg-1ubuntu3.3 [122 kB]
```


Step 3: Additionally, it's a good idea to install npm (Node Package Manager), which is used to install and manage Node.js packages:
```
sudo apt install npm
```

Certainly! Let's break down sudo apt install npm:

sudo: It means "superuser do" and is used to execute the following command with administrative privileges.

apt: Stands for "Advanced Package Tool." It's a package management system used in Ubuntu for handling software packages.

install: This is the sub-command of apt that tells the package manager you want to install a new software package.

npm: This is the specific software package you want to install. In this case, it's the Node Package Manager, used for managing and installing JavaScript packages
```
root@Hunny:/home/vboxuser# sudo apt install npm
Reading package lists... Done
Building dependency tree. Done
Reading state information... Done
The following additional packages will be installed:
git git-man gyp liberror-perl libjs-events libjs-inherits libjs-is-typedarray libjs-psl libjs-source-map libjs-spr
node-abbrev node-agent-base node-ansi-regex node-ansi-styles node-ansistyles node-aproba node-archy node-are-we-the
node-brace-expansion node-builtins node-cacache node-chalk node-chownr node-clean-yaml-object node-cli-table node- node-combined-stream node-commander node-console-control-strings node-copy-concurrently node-core-util-is node-cove
node-delayed-stream node-delegates node-depd node-diff node-encoding node-end-of-stream node-err-code node-escape- node-form-data node-fs-write-stream-atomic node-fs.realpath node-function-bind node-gauge node-get-stream node-glol node-hosted-git-info node-https-proxy-agent node-iconv-lite node-iferr node-imurmurhash node-indent-string node-in node-nopt node-normalize-package-data node-npm-bundled node-npm-package-arg node-npmlog node-object-assign node-onc node-process-nextick-args node-promise-inflight node-promise-retry node-promzard node-psl node-pump node-punycode
node-is-typedarray node-isarray node-isexe node-js-yaml node-jsdom node-json-buffer node-json-parse-better-errors node-lowercase-keys node-lru-cache node-mime node-mime-types node-mimic-response node-minimatch node-minimist node
node-retry node-rimraf node-run-queue node-safe-buffer node-semver node-set-blocking node-signal-exit node-slash no
node-spdx-exceptions node-spdx-expression-parse node-spdx-license-ids node-sprintf-js node-ssri node-stack-utils no
node-supports-color node-tap node-tap-mocha-reporter node-tap-parser node-tar node-text-table node-time-stamp node
node-universalify node-util-deprecate node-validate-npm-package-license node-validate-npm-package-name node-wcwidtl
node-write-file-atomic node-ws node-yallist
Suggested packages:
```


Step 4: Verify that Node.js and npm are installed successfully by checking their versions:
```
node -v
npm - v
```
node -v:
node: This is the command-line interface for Node.js, a JavaScript runtime. It allows you to run JavaScript code outside of a web browser.
-v: This is an option that stands for "version." When you run node -v, it prints out the version of Node.js installed on your system.
In short, node -v tells you the version of Node.js installed on your machine.

npm -v:
npm: Stands for "Node Package Manager." It is a package manager for JavaScript, allowing you to install and manage libraries and frameworks for your Node.js projects.
-v: Similar to the previous example, when you run npm -v, it prints out the version of npm installed on your system.
```
root@Hunny:/home/vboxuser# node -v
v12.22.9
root@Hunny:/home/vboxuser# npm - v
8.5.1
root@Hunny:/home/vboxuser#
```


This should display the installed versions of Node.js and npm, respectively.

Now, you have Node.js and npm installed on your Ubuntu system. You can use them to run JavaScript applications and manage packages.

**Install docsify on ubuntu** 

- To install Docsify on Ubuntu, We can follow these steps. Please note that Docsify requires Node.js to be installed, so make sure you have Node.js installed on your system before proceeding. If you haven't installed Node.js yet, you can refer to the previous answer for instructions.

**Here are the steps to install Docsify:**

Open a terminal on your Ubuntu system.

- Use npm (Node Package Manager) to install Docsify globally. This allows you to use Docsify from any directory:
```
sudo npm install -g docsify -cli
```
sudo: This is a command that stands for "superuser do." It's used to execute the following command with elevated or administrative privileges. It's often required when installing global packages or making system-level changes.

npm: Stands for Node Package Manager. It's a tool for managing and installing JavaScript packages.

install: This is an npm command used to install packages.

-g: This is a flag that stands for "global." It tells npm to install the package globally, making it available system-wide rather than just for the current project.

docsify-cli: This is the name of the package being installed. docsify-cli is the command-line interface for Docsify, a documentation site generator.
```
root@Hunny:/home/vboxuser# sudo npm install -g docsify -cli
added 9 packages, and audited 10 packages in 6s
```


The -g flag installs the package globally.

- Once the installation is complete, you can verify that Docsify is installed by checking its version:
```
 docsify -V
```

Certainly! The docsify -V command is used to check the version of Docsify installed on your system. Let's break it down:

docsify: This is the command you run in the terminal. It is the executable for Docsify, a tool used to generate documentation websites.

-V or --version: This is an option or flag that you provide to the docsify command. When used, it instructs Docsify to display its version number.
```
root@Hunny:/home/vboxuser# docsify -V
docsify-cli version:
  4.4.4 
```


This should display the version number of Docsify.

Now that Docsify is installed, you can use it to initialize a new Docsify project or serve an existing documentation project.

- To create a new Docsify project, navigate to the directory where you want to create your documentation and run:
```
 docsify init ./docs
```
docsify: This is the command-line tool for Docsify.

init: This is a command used to initialize or set up a new Docsify project.

./docs: It specifies the directory where the Docsify project will be initialized. In this case, it's creating a Docsify project in the ./docs directory. You can replace ./docs with the path to your preferred documentation directory.
```
root@Hunny:/home/vboxuser# docsify init ./docs
Initialization succeeded! Please run docsify serve ./docs
```


This command initializes a new Docsify project in the ./docs directory. You can replace ./docs with the path to your preferred documentation directory.

- To preview your Docsify documentation locally, run the following command in the same directory:
```
 docsify serve ./docs
```
docsify: Refers to the Docsify command-line tool.

serve: This is a sub-command of Docsify. When you run docsify serve, it starts a local development server.

./docs: Specifies the directory containing your documentation files. In this case, it's the docs directory in the current location (./).
```
root@Hunny:/home/vboxuser# docsify serve ./docs
Serving /home/vboxuser/docs now. Listening at http://localhost:3000
```

This will start a local development server, and you can view your Docsify documentation by opening your web browser and navigating to
```
<http://localhost:3000>
```
 http://: This is the protocol used for communication between your web browser and the server. It stands for Hypertext Transfer Protocol.

localhost: This is a special hostname that refers to the current device or computer. In this case, it means you are accessing a web server on your own computer.

:3000: This is the port number. Ports are like different doors on a server that handle specific types of communication. In this case, the web server is set to listen on port 3000.

 Deployment (Optional)

To deploy your documentation, upload the contents of the docs folder to your hosting provider. Docsify doesn't require a server, so you can host it on platforms like GitHub Pages, Netlify, or any other static file hosting service.![](https://lh7-us.googleusercontent.com/8kU_bI9lSdullG19t_SdW8fwq-_ys0ZYii45QKJBFZGlgGCAeNvIlPBrtbPAFcnWorcU0Y5pPFdUQp404J9WEjYkOJpLFH69_XaJL8ujzuuyLxChY1PF8-RDBrPXcZHRKfCVWMtYomYj5qND0CE8I4mEaA17Bcn8xGmgObpPToysU23jZmiJXvjLl6q0Rw)

That's it! You've successfully installed and set up Docsify. You can now start adding more content, customize the theme, and explore additional features according to your documentation needs.



