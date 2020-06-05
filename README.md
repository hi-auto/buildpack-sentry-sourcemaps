# buildpack-sentry-sourcemaps

Heroku buildpack to upload sourcemaps to Sentry using `sentry-cli`.

## Usage

Define the following configuration variables within Herkou app. See [Heroku Documentaiton](https://devcenter.heroku.com/articles/config-vars) for more informaiton.

- `SENTRY_AUTH_TOKEN`: the Sentry API authentication token
- `SENTRY_ORG`: the Sentry organization the project lives under
- `SENTRY_PROJECT`: the Sentry project the source maps belong too

## Getting Sentry Auth Token

You can get it on the [API page][]. The token needs the `project:write` scope to be able to upload. The token value would be saved as the `SENTRY_AUTH_TOKEN` configuration variables.

## License

MIT.


[Heroku buildpack]: https://devcenter.heroku.com/articles/buildpacks
[Sentry]: https://sentry.io/
[docs]: https://docs.sentry.io/clients/javascript/sourcemaps/
[API page]: https://sentry.io/api/
