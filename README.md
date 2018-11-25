# path-install

path-install can help you adding a new PATH to .bash_profile and /etc/profile.d/ .

## Installation

    $ gem install path-install
    (you may need to run as root or through sudo.)

## Usage

    $ path-install file or directory...

```
$ path-install /usr/local/ruby2.5.1/bin | tee -a ~/.bash_profile
export PATH=/usr/local/ruby2.5.1/bin:$PATH

$ path-install /usr/local/ruby2.5.1/bin/ruby | sudo tee -a /etc/profile.d/ruby.sh
test -x /usr/local/ruby2.5.1/bin/ruby && \
export PATH=/usr/local/ruby2.5.1/bin:$PATH

```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/s3fxn/path-install.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
