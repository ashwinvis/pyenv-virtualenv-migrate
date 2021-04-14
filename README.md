# pyenv-virtualenv-migrate

pyenv-virtualenv-migrate is a [pyenv](https://github.com/pyenv/pyenv) plugin
to provide a `pyenv virtualenv-migrate` command to migrate all virtual environments from
a Python version to another.

## Installation

### Installing as a pyenv plugin

Installing pyenv-virtualenv-migrate as a pyenv plugin will give you access to the
`pyenv virtualenv-migrate` command.

    git clone https://github.com/pyenv/pyenv-migrate.git $(pyenv root)/plugins/pyenv-migrate
    git clone https://github.com/pyenv/pyenv-virtualenv.git $(pyenv root)/plugins/pyenv-virtualenv
    git clone https://github.com/ashwinvis/pyenv-virtualenv-migrate.git $(pyenv root)/plugins/pyenv-virtualenv-migrate

This will install the latest development version of pyenv-virtualenv-migrate into
the `$(pyenv root)/plugins/pyenv-virtualenv-migrate` directory. From that directory, you
can check out a specific release tag. To update pyenv-virtualenv-migrate, run `git
pull` to download the latest changes.


## Usage

### Using `pyenv virtualenv-migrate` with pyenv

pyenv-virtualenv-migrate uses `pyenv virtualenv` and `pyenv migrate` to
recreate virtual environments with a different Python version. For example, to
migrate virtual environments based on Python `3.8.9` to `3.9.4`, use `pyenv
virtualenv-migrate` as follows:

    pyenv virtualenv-migrate 3.8.9 3.9.4

## Version History

#### 0.0.1

 * Initial release

### License

[(The MIT License)](LICENSE)

* Copyright (c) 2021 Ashwin Vishnu Mohanan
* Copyright (c) 2013-2020 Yamashita, Yuu

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
