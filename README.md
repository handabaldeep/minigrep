# minigrep

Mini version of the classic command line search tool grep written in Rust

## Usage

The tool accepts the following arguments:

1. `query`: We will search for this string.
2. `file_path`: The tool will serach for the `query` string in the contents of this file.

```bash
$ cargo run -- to files/poem.txt
   Compiling minigrep v0.1.0 (file:///projects/minigrep)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.00s
     Running `target/debug/minigrep to files/poem.txt`
Are you nobody, too?
How dreary to be somebody
```

By default the CLI tool will search for case-sensitive matches. To enable case-insensitive search, run the program with `IGNORE_CASE` set to `1`.

```bash
$ cargo run -- to files/poem.txt
   Compiling minigrep v0.1.0 (file:///projects/minigrep)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.00s
     Running `target/debug/minigrep to files/poem.txt`
Are you nobody, too?
How dreary to be somebody!
To tell your name the livelong day
To an admiring bog!
```
