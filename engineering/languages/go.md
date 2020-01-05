# Go

**Why go is not optimal:**

* Pointers
* Lack of immutability
* No algebraic data types
* Imperative paradigm

## Commands

See https://news.ycombinator.com/item?id=20869324
```sh
$ go env -w GOFLAGS=-mod=vendor
$ go env -w GOPROXY="direct"
$ go env -w GOSUMDB="off"
```

## Resources

### Modules

* https://vyskocil.org/blog/go-111-modules-monorepo-and-shared-code/
* https://www.reddit.com/r/golang/comments/9viv50/how_i_solved_go_111_modules_private_monorepo_and/
* https://github.com/go-modules-by-example/index/blob/master/009_submodules/README.md
* https://github.com/sotah-inc/server/tree/master/app
* https://blog.digitalocean.com/cthulhu-organizing-go-code-in-a-scalable-repo/
* https://arslan.io/2019/08/02/why-you-should-use-a-go-module-proxy/

### Other

* https://medium.com/statuscode/how-i-write-go-http-services-after-seven-years-37c208122831
* https://code.tutsplus.com/tutorials/json-serialization-with-golang--cms-30209
* https://eagain.net/articles/go-dynamic-json/
* https://eagain.net/articles/go-json-kind/
* https://arslan.io/2017/09/14/the-ultimate-guide-to-writing-a-go-tool/
* https://tech.labs.oliverwyman.com/blog/2011/04/30/using-the-syntax-tree-in-go/
* https://medium.com/@chemidy/create-the-smallest-and-secured-golang-docker-image-based-on-scratch-4752223b7324
* https://medium.com/@shijuvar/building-microservices-with-event-sourcing-cqrs-in-go-using-grpc-nats-streaming-and-cockroachdb-983f650452aa
* https://ewanvalentine.io/microservices-in-golang-part-10/
* https://blog.golang.org/pipelines
* https://www.gmarik.info/blog/2016/experimenting-with-golang-pipelines/
* https://github.com/trustmaster/goflow
* https://appliedgo.net/flow/
* https://github.com/chrislusf/gleam
* https://fr.slideshare.net/AntonStepanenko/flow-based-programming-in-golang
* https://aws.amazon.com/fr/step-functions/
* https://github.com/Pungyeon/clean-go-article#Introduction-to-Clean-Code
