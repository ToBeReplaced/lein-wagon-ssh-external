# lein-wagon-ssh-external

A Leiningen plugin that enables pulling dependencies and/or deploying
to a repository using `scp`.

This is a minimalist wrapper for:

```clojure
[org.apache.maven.wagon/wagon-ssh-external "2.8"]
```

## Usage

Add the following to your project's `:plugins`:

```clojure
[lein-webdav "0.1.0"]
```

Then, you can use a repository with "scp" as the scheme, like:

```clojure
:repositories {"releases" "scp://maven.company.network/path/to/repository"}
```

## Roadmap

This is currently the bare-minimum implementation, since that is all I
needed for my own network. Adding configuration like custom ssh
arguments is possible in the apache wagon, but not yet implemented
here. I will happily accept pull requests to make this a more
effective wrapper. This will only hit `1.0.0` if that configuration is
complete.

## License

Copyright © 2015 ToBeReplaced

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
