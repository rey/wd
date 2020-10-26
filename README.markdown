# wd

## About

⚠️ This is for educational purposes only -- don't use it for anything serious.

CLI for a subset of the [Wdata API](https://developers.workiva.com/workiva-wdata).

## Dependencies

* curl
* [jq](https://stedolan.github.io/jq)
* wget

## Installation

1. Open `wd` and set the `CLIENT_ID`, `CLIENT_SECRET` and `ENVIRONMENT` variables (Under the `Start here!` bit)
2. 👇

```
ln -s <path to>/wd /usr/local/bin/wd
chmod +x <path to>/wd
```

## Usage

### `wd`

```
Usage: wd <command>

Available Commands:
  wd file         Do stuff with files
  wd table        Do stuff with tables
  wd --version    Show version
  wd --help       Show this message
```

### `wd table`

```
Usage: wd table <command>

Available Commands:
  wd table list               Return all tables available in the workspace
  wd table info <table id>    Return info about the table
  wd table --help             Show this message

```

### `wd file`

```
Usage: wd file <command>

Available Commands:
  wd file list <table id>                       Return all files associated with a table
  wd file info <file id>                        Return info about a file
  wd file upload <table id> <path to file>      Upload a file (append --import to import!)
  wd file delete <file id>                      Delete a file
  wd file download <file id>                    Download a file
  wd file import <table id> <file id>           Import a file
  wd file unimport <table id> <file id>         Unimport a file (append --delete to delete!)
  wd file --help                                Show this message
```
