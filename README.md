###You can use ssed for pipe output of any app to sse clients.

### How to install ssed

```bash
$ go get github.com/mesuutt/ssed
```

### Usage

You can pipe output of any app to clients shown as below:

```bash
$ ./printnumbers.sh | ssed
Reading from STDIN
Listening on  localhost:3000
```

Also you can send messages to clients with a prompt with starting `ssed` with `-p` argument:

```bash
$ ssed -p
Listening on  localhost:3000
(2 clients)-> hello
Sent message: hello
(2 clients)-> how are you?
Sent message: how are you?
```


```
$ ssed -h
Usage of ssed:
  -l string
        Listening address and port (default "localhost:3000")
  -p    Show prompt for message which send to clients

```

