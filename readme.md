# git-label-packages
> Default label packages for [git-label](https://github.com/jasonbellamy/git-label)

Set of reusable Github labels for Bitrock OSS projects, based on the ["Sane Github labeling" principle](https://medium.com/@dave_lunny/sane-github-labels-c5d2e6004b63).

The `bitrock.json` file is simply a merge for the [priority](packages/priority.json), [status](packages/status.json) and [type](packages/type.json) labels schema.

## How to use
Install `git-labelmaker` CLI utility
```bash
$ npm install -g git-labelmaker
-- ora --
$ yarn global add git-labelmaker
```

Clone this repo inside your project, ideally in a git-ignored folder since this operation is a one-shot

```bash
$ git clone https://github.com/bitrockteam/git-label-packages ./node_modules
```

Follows [instruction on git-labelmaker repo](https://github.com/himynameisdave/git-labelmaker#token) for first time setup, then execute it on a project repo:

```bash
$ git-labelmaker
```

To avoid confusion, first select `Remove labels` to delete the default Github ones, then relauch git-labelmaker and now select `Add Labels From Packge` and insert the label schema path:

```
./node_modules/git-label-packages/bitrock.json
```

You're done!


## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality.


## License
Copyright (c) 2018 Bitrock UI Engineering Team & [Jason Bellamy ](http://jasonbellamy.com)  
Licensed under the MIT license.
