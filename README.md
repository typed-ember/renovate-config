# @typed-ember/renovate-config

[![Build Status](https://travis-ci.org/typed-ember/renovate-config.svg?branch=master)](https://travis-ci.org/typed-ember/renovate-config)
[![npm version](https://badge.fury.io/js/%40typed-ember%2Frenovate-config.svg)](https://www.npmjs.com/package/@typed-ember/renovate-config)

Renovate bot sharable config for [typed-ember](https://github.com/typed-ember/) projects.

# What does this do?

- Renovate bot will auto-merge _patch_ and _minor_ releases for most packages
- Human intervention is always required for a _major_ version change of any package
- TypeScript and associated projects that do not follow SemVer require human intervention to update _minor_ versions
- Various packages related to ember-cli and ember addons, with a very low rate of change, are always updated together in a single pull request, rather than treated as individual changes
- versions of `devDependencies` will end up being pinned (see why [here](https://renovatebot.com/docs/dependency-pinning/)). This will only affect library authors, and never consumers of the addon
- `dependencies`, `peerDependencies` and `optionalDependencies` will not be automatically pinned. We don't want to interfere with consumers' ability to use a single dependency version to satisfy multiple libraries

# Legal

&copy; 2018
