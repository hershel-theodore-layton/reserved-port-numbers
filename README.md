`HTL\` projects are becoming Docker Native in Github[^1].
With the aid of `docker-compose.yml`, everyone
should be able to run `git clone https://github.com/...`
and `docker compose up` to get a working development
environment. In order to run side-by-side, these
projects must not step on the port number of a
project next door.

Ports starts at `48544`. This port number was chosen
by converting `HTL` to hex-encoded ASCII. This seemed
like a fitting port number, far away from well-known
ports that might already be in use.
```
\bin2hex('HTL'); // 48544c
```

| Project                                                                                                                     | Linter Port |
| --------------------------------------------------------------------------------------------------------------------------: | :---------- |
| [lecof-router](https://github.com/hershel-theodore-layton/lecof-router)                                                     | 48544       |
| [expect](https://github.com/hershel-theodore-layton/expect)                                                                 | 48545       |
| [expr-dump](https://github.com/hershel-theodore-layton/expr-dump)                                                           | 48546       |
| [hhvm-four-shim](https://github.com/hershel-theodore-layton/hhvm-four-shim)                                                 | 48547       |
| [lecof-router-interfaces](https://github.com/hershel-theodore-layton/lecof-router-interfaces)                               | 48548       |
| [portable-hack-ast](https://github.com/hershel-theodore-layton/portable-hack-ast)                                           | 48549       |
| [portable-hack-ast-extras](https://github.com/hershel-theodore-layton/portable-hack-ast-extras)                             | 48550       |
| [portable-hack-ast-linters](https://github.com/hershel-theodore-layton/portable-hack-ast-linters)                           | 48551       |
| [portable-hack-ast-linters-server](https://github.com/hershel-theodore-layton/portable-hack-ast-linters-server)             | 48552       |
| [pragma](https://github.com/hershel-theodore-layton/pragma)                                                                 | 48553       |
| [sgml-stream](https://github.com/hershel-theodore-layton/sgml-stream)                                                       | 48554       |
| [sgml-stream-codegen](https://github.com/hershel-theodore-layton/sgml-stream-codegen)                                       | 48555       |
| [sgml-stream-interfaces](https://github.com/hershel-theodore-layton/sgml-stream-interfaces)                                 | 48556       |
| [simple-web-token](https://github.com/hershel-theodore-layton/simple-web-token)                                             | 48557       |
| [static-type-assertion-code-generator](https://github.com/hershel-theodore-layton/static-type-assertion-code-generator)     | 48558       |
| [test-chain](https://github.com/hershel-theodore-layton/test-chain)                                                         | 48559       |
| [type-visitor](https://github.com/hershel-theodore-layton/type-visitor)                                                     | 48560       |
| [html-stream-namespaced](https://github.com/hershel-theodore-layton/html-stream-namespaced)                                 | 48561       |
| [html-stream-non-namespaced](https://github.com/hershel-theodore-layton/html-stream-non-namespaced)                         | 48562       |
| [printf-state-machine](https://github.com/hershel-theodore-layton/printf-state-machine)                                     | 48563       |
| [sql-queryf](https://github.com/hershel-theodore-layton/sql-queryf)                                                         | 48564       |
| [sql-queryf-codegen](https://github.com/hershel-theodore-layton/sql-queryf-codegen)                                         | 48565       |
| [json-post-deserialize](https://github.com/hershel-theodore-layton/json-post-deserialize)                                   | 48566       |
| [sgml-stream-exam](https://github.com/hershel-theodore-layton/sgml-stream-exam)                                             | 48567       |

[^1]: I already developed in Docker locally, but
      I created the containers on the fly with
      imperative docker commands. Development was
      always Docker Native, but now also in Github.
