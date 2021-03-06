General
===

> Documentation for general performance metrics.


## Metrics

#### [load.1m](http://linux.die.net/man/5/proc)

The average number of jobs in the run queue (state R) or waiting for disk I/O (state D) over the past minute.

Min | Max | Units | Metric Type | Data Type 
:---: | :---: | :---: | ---: | ---: |
0 | `MAX_FLOAT` | processes and threads | raw | [numeric](https://github.com/doc-metrix/data-types#numeric)


#### [load.5m](http://linux.die.net/man/5/proc)

The average number of jobs in the run queue (state R) or waiting for disk I/O (state D) over the past 5 minutes.

Min | Max | Units | Metric Type | Data Type 
:---: | :---: | :---: | ---: | ---: |
0 | `MAX_FLOAT` | processes and threads | raw | [numeric](https://github.com/doc-metrix/data-types#numeric)


#### [load.15m](http://linux.die.net/man/5/proc)

The average number of jobs in the run queue (state R) or waiting for disk I/O (state D) over the past 15 minutes.

Min | Max | Units | Metric Type | Data Type 
:---: | :---: | :---: | ---: | ---: |
0 | `MAX_FLOAT` | processes and threads | raw | [numeric](https://github.com/doc-metrix/data-types#numeric)


#### [load.running](http://linux.die.net/man/5/proc)

The number of currently running kernel scheduled entities (processes and threads).

Min | Max | Units | Metric Type | Data Type 
:---: | :---: | :---: | ---: | ---: |
1 | `null` | processes and threads | raw | [integer](https://github.com/doc-metrix/data-types#integer)


#### [load.threads](http://linux.die.net/man/5/proc)

The number of kernel scheduled entities (processes and threads) that exist in the system.

Min | Max | Units | Metric Type | Data Type 
:---: | :---: | :---: | ---: | ---: |
0 | `null` | processes and threads | raw | [integer](https://github.com/doc-metrix/data-types#integer)


#### [load.lastPID](http://linux.die.net/man/5/proc)

The process ID (`pid`) of the process that was most recently created on the system.

Min | Max | Units | Metric Type | Data Type 
:---: | :---: | :---: | ---: | ---: |
`null` | `null` | `null` | raw | [integer](https://github.com/doc-metrix/data-types#integer)


#### [uptime](http://linux.die.net/man/5/proc)

The amount of time (in seconds) that the system has been running since the last reboot.

Min | Max | Units | Metric Type | Data Type 
:---: | :---: | :---: | ---: | ---: |
0 | `MAX_FLOAT` | [s](https://github.com/doc-metrix/units#s) | raw | [time](https://github.com/doc-metrix/data-types#time)


===
## Contributing

To contribute to this documentation, see the contributing [guide](https://github.com/doc-metrix/contributing). Any updates to the documentation should be tagged.

``` bash
$ git tag -a <major.minor.patch> -m "[UPDATE] version."
$ git push origin <major.minor.patch>
```

Use [semantic versioning](http://semver.org/) (semvar) for communicating versions.

*	Any new metrics should be communicated as `minor` updates.
*	Any corrections/value modifications should be `patches`.
* 	Any documentation restructuring (changing field names, removing fields, etc) should be communicated as a `major` update.


===
## Usage

The documentation is stored as [JSON](http://json.org/), a lightweight data-interchange format. Many languages provide JSON support: [JavaScript](http://www.json.org/js.html), [Python](https://docs.python.org/2/library/json.html), [Go](http://golang.org/pkg/encoding/json/), [PHP](http://php.net/manual/en/book.json.php), [Java](http://json.org/java/), [Haskell](http://hackage.haskell.org/package/json), and [others](http://json.org/).

You are free to use the JSON documentation, as is. Simply copy the file and use accordingly.

For those using package managers to manage dependencies, we provide package manager support, as outlined below.


### Bower

The documentation is registered as a [Bower](http://bower.io) package. Bower provides a straightforward means for managing dependencies.

In order to use Bower, you must first install [Node.js](http://nodejs.org/) and [Git](http://git-scm.com/book/en/Getting-Started-Installing-Git). Once the prerequisites are installed,

``` bash
$ npm install -g bower
```

To [install](http://bower.io/docs/api/#install) the latest documentation,

``` bash
$ bower install doc-metrix-general
```

Bower will place the documentation in a `bower_components/` directory within the current working directory.

To [update](http://bower.io/docs/api/#update) to the latest documentation,

``` bash
$ bower update doc-metrix-general
```


### Utilities

List of utilities using this documentation:

*	[Node.js Module](https://github.com/doc-metrix/general-node)


---
## License

[MIT license](http://opensource.org/licenses/MIT). 


---
## Copyright

Copyright &copy; 2014. NodePrime.


[git-tag-image]: http://img.shields.io/github/tag/doc-metrix/general.svg
[git-tag-url]: https://github.com/doc-metrix/general/tags

