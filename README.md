# arcanist tools used by the material team

This is a meta-repository that tracks each of the arcanist command line tools used by the material
team.

## Installing the tools

Clone this directory alongside your global arcanist installation:

    cd <folder containing arcanist, libphutil>
    git clone --recursive git@github.com:material-foundation/material-arc-tools.git

## Using the tools

Add each tool you plan to use to your `.arcconfig`'s `load` field:

    {
      "load": [
        "material-arc-tools/arc-proselint",
        "material-arc-tools/arc-hook-conphig",
        "material-arc-tools/arc-hook-github-issues"
      ]
    }

## Updating the tools

Run the following to update each of the tools to their latest stable release:

    git submodule foreach "git fetch;git checkout origin/stable"

## License

Licensed under the Apache 2.0 license. See LICENSE for details.
