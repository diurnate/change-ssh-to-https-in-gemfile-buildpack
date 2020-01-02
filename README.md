# Heroku buildpack

This is a buildpack that you can use if you can't change your requirements.txt file from git@github.com to https://github.com/ paths, but would like to use <https://github.com/timshadel/heroku-buildpack-github-netrc> to access private gems when deploying to heroku.

If you can change your paths to https in requirements.txt manually you probably should. This is for those that can't, or needs to keep the code the way it is until they've fully migrated from an old way of deploying.

## Installing

    heroku buildpacks:add -i 1 https://github.com/diurnate/change-ssh-to-https-in-requirements-txt-buildpack.git
