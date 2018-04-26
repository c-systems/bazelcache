# bazelcache
nginx bazel cache server

.bazelrc

build:remote --spawn_strategy=remote

build:remote --remote_local_fallback

build:remote --genrule_strategy=sandboxed

build:remote --remote_rest_cache=http://localhost:80



run:

bazel build -c opt --config=remote //...
