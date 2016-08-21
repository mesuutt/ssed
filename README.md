###SSE server that you can use for pipe output of any app to sse clients.

You can pipe output of any app to clients:

```bash
$ ./printnumbers.sh | sse
Reading from Stdin
Listening on  localhost:3000
```

Also you can send messages to clients with a prompt with starting sse with `-p` argument:

```bash
$ sse -p
Listening on  localhost:3000
(2 clients)-> hello
Sent message: hello
(2 clients)-> how are you?
Sent message: how are you
```

### Usage

```
Usage of sse:
  -l string
        Listening address and port (default "localhost:3000")
  -p    Show prompt for message which send to clients

```

