# Weave

Weave is a multi-runtime server manager that can host Node.js, Python, Ruby, and Go servers from a single CLI.

## Installation

If you have [knit](https://github.com/Knittight/Knit) installed:

```
knit install weave
```

Or manually:

1. Download `src/weave` to a directory
2. Run `chmod +x src/weave`
3. Run `mv src/weave /usr/local/bin/weave`
4. Run `weave --version` to verify

## Usage

Create a server preset:
```
weave pres -r python server.py
```

Start a server (runtime auto-detected from file extension):
```
weave start -F server.py -p 8000
```

Start a server in daemon mode:
```
weave start -F server.py -p 8000 -d
```

Stop a server (by name or port):
```
weave stop 8000
```

Restart a server:
```
weave restart my_server
```

Check running servers:
```
weave status
```

List supported runtimes:
```
weave list
```
