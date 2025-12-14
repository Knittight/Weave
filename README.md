# Weave

Weave is a server hosting manager that can support node.js, python, and other languages

## Installation

well. if you have (knit)[https://github.com/Knittight/Knit] installed, you can just do `knit install weave` thats it.

buut if you wanna be extra i can say this

1. Download src/weave to a folder for example... "qwert"
2. Run `chmod +x qwert/src/weave`
3. Run `mv qwert/src/weave /usr/local/bin/weave`
4. Run `weave --version` to check if it works.

## Usage

To make a server preset run `weave pres -r <runtime> <file>`
To run said server preset run `weave start -r <runtime> -F <file> -p <port>`
To stop said server run `weave stop <port>`
To list all servers run `weave status`