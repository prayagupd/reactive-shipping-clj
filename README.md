# reactive-shipping

designed to ship packages to customer

![](https://drive.google.com/uc?id=0B9FyLOsn9I34anV4UFJQTWZLYnc)


## Usage

- install `lein`
- setup `~/.lein/profiles.clj` in case of proxy

```
{:user                                                                                                                                               {:repository [["artifactory-libs-releases" "https://code.shipping.com/artifactory/libs-release/"]        
                ["artifactory-libs-snapshot" "https://code.shipping.com/artifactory/libs-snapshot/"]]} 
}
```


```
$ lein run inline < input-events > output-events

;; or 

$ lein run async < input-events
(async)
package-1 shipped
package-2 shipped
package-4 shipped
package-7 shipped
package-5 shipped
package-6 shipped
package-3 shipped
package-8 shipped
package-13 shipped
package-9 shipped
package-14 shipped
package-15 shipped
package-11 shipped
package-16 shipped
...
```

## License

Copyright © prayagupd

##  References

[Chapter 9 - The Sacred Art of Concurrent and Parallel Programming](http://www.braveclojure.com/concurrency/)

[Chapter 11 - Mastering Concurrent Processes with core.async](http://www.braveclojure.com/core-async/)

[Using core.async for Producer-consumer Systems
](http://elbenshira.com/blog/using-core-async-for-producer-consumer-workflows/)
