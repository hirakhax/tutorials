# Install Ruby And Rails on Fedora 36

## Install Prerequisists
```
sudo dnf install git-core zlib zlib-devel gcc-c++ patch readline readline-devel libyaml-devel libffi-devel openssl-devel make bzip2 autoconf automake libtool bison curl sqlite-devel
```

## Install rbenv

Clone `rbenv` repository to `.rbenv` directory
```
git clone https://github.com/sstephenson/rbenv.git .rbenv
git clone https://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
```

Add `rbenv` path in `.bashrc`
```
sudo nano ~/.bashrc
```

Add this line in `.bashrc` file before `unset rc`
```
export PATH="$HOME/.rbenv/bin:$PATH"
export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"
```

Now restart your pc/laptop.

## Install Ruby
List the available Ruby versions for your system using the following command.
```
rbenv install -l
```

```
rbenv install 3.1.2
```

```
rbenv global 2.4.2
```
 
```
ruby -v
```
If this command not showing ruby version, then restart your pc and then try this command.


## Install Rails
```
gem install rails
```

Install additional gems
```
gem install bundler
gem install ffi
gem install bindex
``
