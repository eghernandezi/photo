name: Simple Usage

on: push

jobs:
  convert_via_pandoc:
    runs-on: ubuntu-18.04
    steps:
      - uses: docker://pandoc/core:2.9
        with:
          args: "--help" # gets appended to pandoc command
