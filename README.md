# buildpack-null

A buildpack that performs no actions, for testing purposes

> WARNING: This buildpack performs no actions, and is strictly for testing purposes. Do not use unless your app vendors all it's own dependencies.

## Usage

To use, you need to specify the buildpack like so:

```
# via command
dokku buildpacks:set $APP https://github.com/dokku/buildpack-null

# via env var
dokku config:set $APP BUILDPACK_URL=https://github.com/dokku/buildpack-null

# via a .buildpacks file with the following contents
https://github.com/dokku/buildpack-null
```

Next, your repository will need a file called `null` in the root. The buildpack will be in use if you complete these two steps.
