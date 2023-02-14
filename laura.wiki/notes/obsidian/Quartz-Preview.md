---
title : "Quartz Preview"
feed: show
date : 02-08-23
tags : -quartz
---

To enable a local live preview of the static site that is generated from the local Obsidian vault, follow the steps [here](https://quartz.jzhao.xyz/notes/preview-changes/).  A confusing detail is that this live preview is required for all backlinks and graphs to work properly. Details below..

1. Install GO
	1. [GO](https://go.dev/doc/install)
	2. Verify GO is installed by typing in the following to cmd
	3. `$ go version`
2. Install Hugo-Obsidian
	1. Use cmd
	2. `go install github.com/jackyzha0/hugo-obsidian@latest`
3. Install Hugo GO
	1. https://gohugo.io/installation/
		1. Open up an Administrative Powershell
		2. Install [choco](https://chocolatey.org/)
		3. `choco install hugo-extended`
4. CD into working github directory
5. Use HUGO to build site and serve locally
	1. make serve
	2. manual hugo commands
		1. `hugo-obsidian -input=content -output=assets/indices -index -root=.`
		2. ` hugo server --enableGitInfo --minify --bind=0.0.0.0 --baseURL=http://localhost --port=1313 --appendPort=true --liveReloadPort=-1`
6. Editing GOPATH (May or may not be required)
	1. Enter these commands every time you restart the server
	2. `export GOPATH=$HOME/go`
	3. `export PATH=$PATH:$GOROOT/bin:$GOPATH/bin`
	4. ![Screenshot](notes/images/GOPATH.png)