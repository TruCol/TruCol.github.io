# TruCol


## Contributing

Contributions are welcome. Feel free to open a pull request with changes.

### Run Website Locally - Instructions

It can be helpful to preview changes on your computer before opening a pull request. *The Markdown Guide* uses the [Jekyll static site generator](http://jekyllrb.com/). After forking or cloning the repository, perform the following steps to generate the site and preview it:

- Make sure you have ruby installed on your computer. See https://www.ruby-lang.org/en/downloads/
- `bundle install`
- `bundle exec jekyll serve`
- Browse to: http://127.0.0.1:4000/

### Run Website Locally - Ubuntu Commands
```
# Source: https://rvm.io/
yes | sudo apt install gnupg2
gpg2 --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
\curl -sSL https://get.rvm.io | bash -s stable
\curl -sSL https://get.rvm.io | bash -s stable --rails
yes | sudo apt  install ruby-bundler
yes | sudo apt install ruby-dev
git clone git@github.com:TruCol/TruCol.github.io.git
cd TruCol.github.io
bundle install

# Run the website locally with:
bundle exec jekyll serve
```

## Deployment

Pull requests merged to the master branch are automatically deployed to the production website.

## License

The content of this project itself is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International license](https://creativecommons.org/licenses/by-sa/4.0/), and the underlying source code used to format and display that content is licensed under the [MIT license](LICENSE.txt).
