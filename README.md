# Jekyll Tempalte

A static site template to jumpstart your next JAM stack project. Built with Jekyll and Materialize CSS.

### Quick Start

- For system setup instructions, see [Install Doc](./docs/install.md)

```
$ rvm use 2.2.3
$ yarn  # First set up only
$ bundle install  # first set up only
$ jekyll serve
```

### Create a new repo mirroring this one

- Create a new repo that isn't initialized.
- Clone this repo

```bash
$ git clone --bare https://github.com/swoloszynski/jekyll-template.git
```

- Mirror push to the new repo.

```bash
$ cd old-repository.git
$ git push --mirror https://github.com/exampleuser/new-project.git
```

- Remove the clone of the template repo.

```bash
$ cd ..
$ rm -rf jekyll-template.git
```

- Clone the new repo.

```bash
$ git clone git@github.com:swoloszynski/new-project.git
```


### Tests

Travis CI runs `scripts/cibuild`.

[HTML Proofer](https://github.com/gjtorikian/html-proofer) lints the html files.

To exclude an HTML tag from checks, add `data-proofer-ignore` as an attribute.
