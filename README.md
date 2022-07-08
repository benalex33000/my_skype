# My_skype

This is a copy of skype coding in cpp.


This project was split into two main part

The first part is the skype backend and the second is the client version.
## Installation

You have to install [CMake](https://cmake.org/install/)

```bash
./autobuild.sh
```

If you want to generate the compile_commands.json 

```bash
./autobuild.sh cc
```

## Usage
### You need to run two binary :
#### Server:
```bash
./skype-server <port>
```
#### Client:
```bash
./skype-client <port>
```

## Naming Conventions

# Branch naming convention

Branches names should look like this:

`<issue-number>_<parent-branch>_<issue-summary>`

## Convention

### `issue-number`

The ID of the issue the branch is created for work on

### `parent-branch`

The name of the branch this branch will be merged to (and often is created from)

It is often the 'category' of the work

### `issue-summary`

The summary of the issue the branch is created for

## Examples

### Branch to do #13 issue and is from `Arduino` branch to create a clock

`13_Arduino_Create-clock`

### Branch to do #7 issue and is from `UI` branch to create auth page

`7_UI_Create-auth-page`

# Commit convention

Commits should look like this:

`<type>([scope]): <description> [#<issue-number>]`

`[body]`

## Convention

### `type`

The type if the classification of the modification you are commiting

For example, if you are adding a new functionality it will be `feat`

If you are solving a bug it will be `fix`

Here is a list of `type` keyword

- `feat`: adding of a new functionality / new library
- `fix`: Resolving a problem (bug, wrong display)
- `doc`: Adding new documentation
- `refact`: Refacting a part of code / all the code
- `test`: Adding tests
- `improvement`: Upgrading an existing functionality

### `scope`

The scope is optionnal, it's an indication of the part of code / functionality your commiting into

For exemple, if you're adding a ci you can use: `feat(ci)`

### `description`

The description is a brief text that describe what you are committing

### `issue-number`

The issue number allows linking your commit to an issue

It is also on what part of the code you're working

### `body`

The body is an optionnal additionnal information to add supports (links, images, ...)

Or just describe in details the problem you are fixing / you find

## Examples

### Commiting a new language on an application

`feat(language): Adding of the russian language #14`

`Adding the russian option for the translation of the home page`

### Commiting a bugfix

`fix(keyboard): Removing the blinking effect when pressing keys #54`

### Commiting new tests

`test(authentication): Adding full test on the authentication`


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
