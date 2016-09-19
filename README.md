###You can use ssed for pipe STDOUT of any command-line program to SSE clients.


#### How to install ssed?

```bash
$ go get github.com/mesuutt/ssed
```

### Usage

You can pipe STDOUT of any command-line program to ssed for send output 
of the program to the SSE clients:

```bash
$ ./printEverySecond.sh | ssed
Reading from STDIN
Listening on  localhost:3000
```

Also you can send messages to SSE clients with a prompt with starting `ssed` with `-p` argument:

```bash
$ ssed -p
Listening on  localhost:3000
(1 clients)-> hello
Sent message: hello
(1 clients)-> how are you?
Sent message: how are you?
```


```
$ ssed -h
Usage of ssed:
  -l string
        Listening address and port (default "localhost:3000")
  -p    Show prompt for message which send to clients

```

