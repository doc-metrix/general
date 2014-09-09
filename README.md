General
===

> A specification for general performance metrics.


## Metrics

#### [load.1M](http://linux.die.net/man/5/proc)

The average number of jobs in the run queue (state R) or waiting for disk I/O (state D) over the past minute.

Min | Max | Units | Metric Type | Data Type 
:---: | :---: | :---: | ---: | ---: |
0 | `MAX_FLOAT` | processes and threads | raw | [numeric](https://github.com/doc-metrix/data-types#numeric)


#### [load.5M](http://linux.die.net/man/5/proc)

The average number of jobs in the run queue (state R) or waiting for disk I/O (state D) over the past 5 minutes.


#### [load.15M](http://linux.die.net/man/5/proc)

The average number of jobs in the run queue (state R) or waiting for disk I/O (state D) over the past 15 minutes.


#### [load.running](http://linux.die.net/man/5/proc)

The number of currently running kernel scheduled entities (processes and threads).

Note: the minimum value for this metric is 1, if we assume that the process monitoring the metric is counted.


#### [load.threads](http://linux.die.net/man/5/proc)

The number of kernel scheduled entities (processes and threads) that exist in the system.


#### [load.lastPID](http://linux.die.net/man/5/proc)

The process ID (PID) of the process that was most recently created on the system.


#### [uptime](http://linux.die.net/man/5/proc)

The amount of time (in seconds) that the system has been running since the last reboot.


===
## Contributing

To contribute to this specification, see the contributing [guide](https://github.com/doc-metrix/contributing). Any updates to the specification should be tagged.

``` bash
$ git tag -a <major.minor.patch> -m "[UPDATE] version."
$ git push origin <major.minor.patch>
```

Use [semantic versioning](http://semver.org/) (semvar) for communicating versions.

*	Any new metrics should be communicated as `minor` updates.
*	Any corrections/value modifications should be `patches`.
* 	Any specification restructuring (changing field names, removing fields, etc) should be communicated as a `major` update.


===
## Usage

The specification is stored as [JSON](http://json.org/), a lightweight data-interchange format. Many languages provide JSON support: [JavaScript](http://www.json.org/js.html), [Python](https://docs.python.org/2/library/json.html), [Go](http://golang.org/pkg/encoding/json/), [PHP](http://php.net/manual/en/book.json.php), [Java](http://json.org/java/), [Haskell](http://hackage.haskell.org/package/json), and [others](http://json.org/).

You are free to use the JSON specification, as is. Simply copy the file and use accordingly.

For those using package managers to manage dependencies, we provide package manager support, as outlined below.


### Bower

The specification is registered as a [Bower](http://bower.io) package. Bower provides a straightforward means for managing dependencies.

In order to use Bower, you must first install [Node.js](http://nodejs.org/) and [Git](http://git-scm.com/book/en/Getting-Started-Installing-Git). Once the prerequisites are installed,

``` bash
$ npm install -g bower
```

To [install](http://bower.io/docs/api/#install) the latest specification,

``` bash
$ bower install doc-metrix-general
```

Bower will place the specification in a `bower_components/` directory within the current working directory.

To [update](http://bower.io/docs/api/#update) to the latest specification,

``` bash
$ bower update doc-metrix-general
```


### Utilities

List of utilities using this specification:

*	[Node.js Module](https://github.com/doc-metrix/general-node)


---
## License

[MIT license](http://opensource.org/licenses/MIT). 


---
## Copyright

Copyright &copy; 2014. NodePrime.

