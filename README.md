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

| Project                                                                 | Linter Port |
| ----------------------------------------------------------------------: | :---------- |
| [lecof-router](https://github.com/hershel-theodore-layton/lecof-router) | 48544       |

[^1]: I already developed in Docker locally, but
      I created the containers on the fly with
      imperative docker commands. Development was
      always Docker Native, but now also in Github.
