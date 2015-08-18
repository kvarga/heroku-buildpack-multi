# heroku-buildpack-multi

Use multiple buildpacks on your app

## Usage

    $ heroku buildpacks:set https://github.com/ddollar/heroku-buildpack-multi.git

    $ cat .buildpacks
    https://github.com/heroku/heroku-buildpack-nodejs.git#0198c71daa8
    https://github.com/heroku/heroku-buildpack-ruby.git#v86

## Comments

You can use # at the beginning of lines to leave a comment. For example

    $ cat .buildpacks
    # Buildpacks File

    # Node Buildpack set at specific commit to avoid regression issue in issue 42
    https://github.com/heroku/heroku-buildpack-nodejs.git#0198c71daa8

    # Ruby Buildpack for scheduled jobs
    https://github.com/heroku/heroku-buildpack-ruby.git#v86

## License

MIT
