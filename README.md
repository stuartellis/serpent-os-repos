# serpent-os-repos

Repositories for Serpent OS.

This collection uses the [mani](https://manicli.com/) repository manager.

## Setup

The mani command-line tool is a single executable file.

To install mani, either use Homebrew, or fetch the current release from [the releases on GitHub](https://github.com/alajmo/mani/releases). If you download the tool manually, ensure that you set the permissions on the file as executable.

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
