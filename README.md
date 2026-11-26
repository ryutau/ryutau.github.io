# ryutau.github.io

## Local preview

Install the project Ruby once:

```sh
brew install ruby@3.3
```

Install the dependencies:

```sh
export PATH="/opt/homebrew/opt/ruby@3.3/bin:/opt/homebrew/lib/ruby/gems/3.3.0/bin:$PATH"
gem install bundler -v 4.0.16 --no-document
bundle config set --local path vendor/bundle
bundle install
```

Then start the local site:

```sh
./bin/serve
```

Open <http://localhost:4000/> or <http://localhost:4000/jp>.

## Local build

After installing the dependencies, build the static site:

```sh
./bin/build
```

The generated site is written to `_site/`.
