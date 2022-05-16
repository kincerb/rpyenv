# Research info

## python packages

### cloudpickle

[cloudpickle](https://pypi.org/project/cloudpickle/) makes it possible to serialize Python constructs not
supported by the default `pickle` module.

It's especially useful for *cluster computing* where python code is shipped over the network to execute on
remote hosts.

### msgpack

[MessagePack](https://pypi.org/project/msgpack/) is a binary serialization format. It's supposed to be smaller
and faster than JSON.

Example:

```python
>>> import msgpack
>>> msgpack.packb([1, 2, 3], use_bin_type=True)
'\x93\x01\x02\x03'
>>> msgpack.unpackb(_, raw=False)
[1, 2, 3]
```

### tblib

[tblib](https://pypi.org/project/tblib/) is a serialization library for Exceptions and Tracebacks.

## Serverless projects

### Fn Project

[fn project](https://fnproject.io) is a do-it-yourself serverless solution. Supports all the runtimes.

### fission

[Fission](https://github.com/fission/fission) is a serverless framework for Kubernetes.
