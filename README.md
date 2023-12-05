# Julia for HPC @ UCL 2024 website

This is the source code of [Julia for HPC @ UCL 2024](https://github-pages.arc.ucl.ac.uk/julia-hpc-2024/) website, based on the
[`jekyll-theme-conference`](https://github.com/DigitaleGesellschaft/jekyll-theme-conference) theme.

## Building the website

### On GiThub

The website is automatically built and deployed upon pushes to this branch.

### Locally

If you want to build locally the website for testing, install Jekyll

```sh
gem install jekyll bundler
```

and then

```sh
bundle exec jekyll build --watch
```

to build the website.  The `--watch` option automatically rebuilds the website
if there are changes to the source code, but it won't reflect changes to the
configuration file `_config.yml`.  Note that `--watch` keeps the process alive
to update the project.

Then, you can start a server to view the website with

```sh
python3 -m http.server -d _site
```

and open the displayed URL (by default it should be <http://0.0.0.0:8000/>).

## License

This project is licensed under the MIT License. You can view [LICENSE.md](LICENSE.md) for more details.

This project redistributes other opensource tools and libraries. You can view [REDISTRIBUTED.md](REDISTRIBUTED.md) for third party licenses.
