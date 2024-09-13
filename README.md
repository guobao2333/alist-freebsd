# alist-freebsd
[![Build Alist](https://github.com/guobao2333/alist-freebsd/actions/workflows/build.yml/badge.svg)](https://github.com/guobao2333/alist-freebsd/actions/workflows/build.yml)

Automatically build alist every night (FreeBSD version)

It seems many people use this project as a template to build apps for FreeBSD.

Actually, in most situations, this will be not neccessary.

Only apps that requires cgo (like alist) are needed to use a native FreeBSD environment to build, as currently no reliable C cross-compiler for BSD platform exists.

If the app is written in pure Go (and has no cgo depenencies), you can simply using the `go` tool with GOOS=freebsd variable to build a FreeBSD binary.
