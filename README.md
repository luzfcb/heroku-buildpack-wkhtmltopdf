# Heroku Buildpack: wkhtmltopdf

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for using [wkhtmltopdf](http://wkhtmltopdf.org/) in your application.


## Usage

    $ heroku buildpacks:add --index 1 https://github.com/luzfcb/heroku-buildpack-wkhtmltopdf.git

Deploy your applicatio.

    $ git push heroku master

Remember to clean your repository cache if you are updating the version of buildpack. To do that, run:

    $ heroku plugins:install https://github.com/heroku/heroku-repo.git
    $ heroku repo:purge_cache -a appname

You can verify that everything is properly installed by running the following command:

    $ heroku run "wkhtmltopdf -V"

The output should be:

    wkhtmltopdf 0.12.4 (with patched qt)

## Issues

If you have problems, please create a [Github Issue](https://github.com/rafaelp/heroku-buildpack-wkhtmltopdf/issues).

## Credits

heroku-buildpack-wkhtmltopdf was originally written by [Rafael Lima](http://rafael.adm.br).

Working at [Boleto Simples](https://boletosimples.com.br)

Github: [http://github.com/rafaelp](http://github.com/rafaelp)

Twitter: [http://twitter.com/rafaelp](http://twitter.com/rafaelp)

## License

heroku-buildpack-wkhtmltopdf is Copyright © 2014 Rafael Lima. It is free software, and may be redistributed under the terms specified in the [LICENSE](https://github.com/rafaelp/heroku-buildpack-wkhtmltopdf/blob/master/LICENSE) file.
