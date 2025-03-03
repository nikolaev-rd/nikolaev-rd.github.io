<!-- markdownlint-disable MD041 -->
[![Pages Deploy](https://github.com/nikolaev-rd/nikolaev-rd.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/nikolaev-rd/nikolaev-rd.github.io/actions/workflows/pages/pages-build-deployment)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fnikolaev-rd%2Fnikolaev-rd.github.io&count_bg=%2379C83D&title_bg=%23555555&title=👀)](https://hits.seeyoufarm.com)

# [CV](https://ru.wikipedia.org/wiki/Curriculum_vitae) site

This static site is builded on [Jekyll](https://jekyllrb.com/) and theme from Xiaoying Riley ([3rd Wave Media](https://themes.3rdwavemedia.com/)).

## Configuration

- Jekyll configuration for site: [`_config.yml`](./_config.yml)
- CV:
  - data structure: [_data/data.yml](./_data/data.yml)
  - labels renaming: [_data/labels.yaml](./_data/labels.yaml)

## Launch

Local site & linters can be launched via [Docker Compose](https://docs.docker.com/compose/).

### Prepare

Install [Docker Desktop](https://docs.docker.com/desktop/) (Docker Engine & Docker Compose — already included).

Then your can change (if needed) variables for [docker-compose.yml](./docker-compose.yml) services in [`.env`](./.env).

### Launch Site

- Run site via Docker Compose: `make site` or just `make`
- Open you site: <http:/localhost:4000/>

## Linters

Run all linters: `make lint`

### YAML lint

- Run [yamllint](https://yamllint.readthedocs.io/en/stable/) via Docker Compose: `make yaml-lint`

### Launch HTML Proofer

- Run [HTML Proofer](https://github.com/gjtorikian/html-proofer) via Docker Compose: `make html-proofer`
- Check output errors (if exist) and fix it!

## Credits

- This theme is designed by Xiaoying Riley at [3rd Wave Media](https://themes.3rdwavemedia.com/)
- [Font Awesome](https://use.fontawesome.com/releases/v6.4.2/fontawesome-free-6.4.2-web.zip)

## License

This project is licensed under the [MIT license](./LICENSE.txt).
