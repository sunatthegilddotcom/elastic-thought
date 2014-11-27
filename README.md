
REST API wrapper for the [Caffe](caffe.berkeleyvision.org) deep learning framework.

## Quick Start

# Install go1.3 or later

```

```

# Start Nsq

```
$ nsqlookupd & 
$ nsqd --lookupd-tcp-address=127.0.0.1:4160 &
$ nsqadmin --lookupd-http-address=127.0.0.1:4161 &
```

# Start Sync Gatewway

```
$ ./run.sh config.json
```

# Start httpd

# Start cbfs

# Start Couchbase Server





## Architecture

It uses the following components for storing data / blobs:

* [Couchbase Server](http://www.couchbase.com/nosql-databases/couchbase-server)
* [Sync Gateway](https://github.com/couchbase/sync_gateway) 
* [CBFS](https://github.com/couchbaselabs/cbfs)

Under construction.

## Todo

- Validate solver.prototxt: 
  - it should assert "net" arg is empty
  - the worker should rewrite the solver_mode CPU/GPU based on worker capabilities 

