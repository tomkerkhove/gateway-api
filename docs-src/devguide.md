<!--
Copyright 2019 The Kubernetes Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

# Building, testing and deploying

You will need to have Docker installed to perform the steps below.

## Building the code

TODO

## Testing the code

TODO

## Documentation

The site documentation is written in [mkdocs][mkdocs] format. The files are
contained in `docs/`.

Building the docs:

```shell
make -f docs.mk
```

Live preview for editing (view on [http://localhost:8000]()):

```shell
make -f docs.mk serve
```

### Publishing

We currently publish the docs using Github pages
(https://kubernetes-sigs.github.io/service-apis/). Submit a PR against the
`gh-pages` branch, where the root of the repository is the contents of the
`/site/` produced by the doc build.

TODO(bowei): this is pretty awkward and I think we should just have the docs
TODO(bowei): in the master branch.

[mkdocs]: https://www.mkdocs.org/