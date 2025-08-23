# Seattle Systems

This is a [Jekyll](https://jekyllrb.com/) site hosted on [GitHub Pages](https://pages.github.com/).

Site url: [www.seattlesystems.xyz](https://www.seattlesystems.xyz)

## Requirements

* [Ruby](https://www.ruby-lang.org/en/downloads/)
* [Bundler](https://bundler.io/)

## Running locally

1. **Clone the repository**

   ```bash
   git clone https://github.com/spattk/seattle-systems.git
   cd seattle-systems
   ```

2. **Install dependencies**

   ```bash
   bundle install
   ```

3. **Run the development server**

   ```bash
   bundle exec jekyll serve
   ```

   The site will be available at:

   ```
   http://localhost:4000
   ```

4. **Stop the server**
   Press `CTRL + C` in your terminal.

## Troubleshooting Local Development on macOS

1. **Install ruby**
   ```
   brew install rbenv ruby-build
   rbenv install 3.2.2
   rbenv global 3.2.2
   ```

2. **Check ruby version** (>= 3.2.2)
   ```
   ruby -v
   eval "$(rbenv init -)"
   ```


3. **Add rbenv to bashrc/zshrc**
   ```
   echo 'eval "$(rbenv init -)"' >> ~/.zshrc
   ```

## Deployment on GitHub Pages

* This site is configured to run automatically on GitHub Pages.
* You **do not** need to build the site manually for deployment—GitHub Pages will install the necessary gems and build the site on its servers.
* Make sure your repository is set to use the correct branch and folder in **Settings → Pages**.

## Project structure

```
.
├── _config.yml       # Jekyll configuration
├── Gemfile           # Ruby gems list
├── Gemfile.lock      # Locked gem versions
├── _data/
  └── events.yml      # List of past and upcoming events (site only displays future events)
├── images/
  ├── favicon.ico     # Used for site favicon
  ├── logo_small.png  # Minimalist version of logo embedded in the site
  └── logo.png        # Full version of logo used for social links
├── CNAME             # Domain configuration
├── index.html        # Site html
└── styles.css        # Site css
```

## Included gems

* `jekyll` – Static site generator
* `csv` – data parsing
* `base64` – Base64 encoding/decoding
* `tzinfo` / `tzinfo-data` – Time zone handling
