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


## Guides

### How to access a SQL Database

comment acceder a la db

pq orm: https://github.com/go-pg/pg
postgres driver: https://github.com/go-pg/pg
sqlx: https://github.com/jmoiron/sqlx (pas mis a jour)
gorm: https://github.com/jinzhu/gorm



ce qui semble se dessiner:
sqlx, avec repository pattern, comme ca on peut switcher / alterner

pattern

domain
- mode
- command (ou use cases?)
- query (repositories?)
handler

et les repositories ?


on met la logique ‘gloable’ dans les handler, et ceux ci ne font que appeler des groupement de commandes




he file service.go represents the Use Case layer, as defined by Uncle Bob. In the file we have the interface Service and his implementation. The Service interface is:

———————

les handler sont nos controller

dans le domaine on retrouve les commandes, les notifs et les modeles




## Resources

### Modules

* https://vyskocil.org/blog/go-111-modules-monorepo-and-shared-code/
* https://www.reddit.com/r/golang/comments/9viv50/how_i_solved_go_111_modules_private_monorepo_and/
* https://github.com/go-modules-by-example/index/blob/master/009_submodules/README.md
* https://github.com/sotah-inc/server/tree/master/app
* https://blog.digitalocean.com/cthulhu-organizing-go-code-in-a-scalable-repo/
* https://arslan.io/2019/08/02/why-you-should-use-a-go-module-proxy/

### CGO

* https://gist.github.com/helinwang/2c7bd2867ea5110f70e6431a7c80cd9b
* https://golang.org/cmd/cgo/
* https://blog.golang.org/c-go-cgo
* https://stackoverflow.com/questions/35507467/cgo-how-to-free-memory-allocated-in-c-using-malloc-from-go-to-avoid-memory-leak
* https://karthikkaranth.me/blog/calling-c-code-from-go/
* https://dave.cheney.net/tag/cgo
* http://akrennmair.github.io/golang-cgo-slides/#1

### Other

* https://yourbasic.org/golang/switch-statement/
* https://www.yellowduck.be/posts/injecting-build-time-variables/
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
