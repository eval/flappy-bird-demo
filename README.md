# flappy-bird-demo

Read the [blog post](http://rigsomelight.com/2014/05/01/interactive-programming-flappy-bird-clojurescript.html) about this flappy bird demo.


```
(setq cider-cljs-lein-repl "(do (use 'figwheel-sidecar.repl-api) (start-figwheel!) (cljs-repl))")
```

Docker image:
```
function demacs() {
  path=$(pwd)
  name=${path##*/}
  docker run -it --rm --name "emacs-${name}" -p 3449:3449 -p 3450:3450 -v ${path}:/root/project registry.gitlab.com/eval/docker-lein-emacs:cider-0.14.0 /bin/bash -c "[[ -f /root/project/.envrc ]] && source /root/project/.envrc;emacs /root/project/${1}"
}
```

Watch the 6 minute [video](https://www.youtube.com/watch?v=KZjFVdU8VLI)

Checkout the documentation on [lein-figwheel](https://github.com/bhauman/lein-figwheel) to go further!

## License

Copyright © 2014 Bruce Hauman

Distributed under the [Eclipse Public License](LICENSE) either version 1.0 or any
later version.
