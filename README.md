# kxss

[1.1]: http://i.imgur.com/tXSoThF.png
[1]: https://twitter.com/TobiunddasMoe

This is an adaptation of tomnomnom's kxss tool with a different output format. I didn't want to fork his whole Hacks repository, so I created my own.

All credit for the original code goes to [Tomnomnom](https://github.com/tomnomnom/).

## Changes to original kxss

The output format is easier to grep in recon scripts:

```text
URL: https://www.example.com/event_register.php?event=177 Param: event Unfiltered: [" ' < >]
```

## Installation

Install the latest released version with Go:

```sh
go install github.com/Emoe/kxss@latest
```

Make sure Go's binary directory is in your `PATH`. By default this is:

```sh
export PATH="$PATH:$(go env GOPATH)/bin"
```

To build from a local checkout instead:

```sh
go install .
```

## Usage

Pipe URLs into `kxss`:

```sh
echo "https://www.example.com/event_register.php?event=177" | kxss
```

## Questions

If you have a question, you can create an issue or ping me on [![alt text][1.1]][1].
