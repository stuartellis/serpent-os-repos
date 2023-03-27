# serpent-os-repos

Repositories for [Serpent OS](https://github.com/serpent-os).

This collection uses the [mani](https://manicli.com/) repository manager.

## Setup

The [mani](https://manicli.com/) command-line tool is a single executable file.

To install mani, either use [Homebrew](https://github.com/alajmo/mani#installation), or fetch the latest  release from [the releases on GitHub](https://github.com/alajmo/mani/releases).

Follow these commands to install mani on a Linux system from GitHub:

    # Replace 0.23.0 on this line with latest version of mani from https://github.com/alajmo/mani/releases
    export MANI_VERSION=0.23.0

    mkdir -p $HOME/bin
    curl -L https://github.com/alajmo/mani/releases/download/v$MANI_VERSION/mani_$MANI_VERSION_linux_amd64.tar.gz > mani.tar.gz
    tar xvzf mani.tar.gz
    cp mani $HOME/bin
    rm mani* LICENSE

## Usage

To see the projects that mani is configured to track, run *mani list projects*:

    mani list projects

To clone all of the repositories for the projects, run *mani sync*:

    mani sync

> *Clones are automatically excluded from version control:* The *sync* command adds each repository that it clones to the *.gitignore* file.

To see the available tasks, run *mani list task*:

    mani list task

To run a task:

    # Run task <task> for all projects
    mani run <task> --all

    # Run task <task> for all projects <project>
    mani run <task> --projects <project>

    # Run task <task> for all projects that have tags <tag>
    mani run <task> --tags <tag>

## License

Refer to the LICENSE file for the license on the unique content for this repository.

Refer to the LICENSE files in the managed repositories for licensing of the content of those repositories.
