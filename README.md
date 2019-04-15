# Issues

GitHub Issues app is my implementation of example app from
"Programming Elixir" book. As the book got outdated with the time, I adapted
code for modern libraries versions when I was writing the code.

## Setup

Clone, get deps, etc.

```bash
git clone https://github.com/cr0t/issues.git
cd issues/
mix deps.get
```

## Run It

You can run it via mix ability to eval the code:

```bash
mix run -e 'Issues.CLI.main(["elixir-lang", "elixir", "1"])'

20:06:40.380 [info]  Fetching user elixir-lang's project elixir

20:06:44.209 [info]  Successful response
numb | created_at           | title
-----+----------------------+--------------------------------------------------------
6248 | 2017-06-22T09:41:01Z | Improve ExUnit output for assertions on process mailbox
```

Or you can build a single binary file and execute it directly:

```bash
mix escript.build
./issues elixir-lang elixir 2

20:06:40.380 [info]  Fetching user elixir-lang's project elixir

20:06:44.209 [info]  Successful response
numb | created_at           | title
-----+----------------------+--------------------------------------------------------
6248 | 2017-06-22T09:41:01Z | Improve ExUnit output for assertions on process mailbox
6611 | 2017-09-28T08:56:29Z | Support Erlang 21 new features
```
