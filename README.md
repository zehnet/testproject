# Welcome


## __construct
creates an StreamInterface instance

```php
__construct($stream = '', array $options = array(), \React\Stream\WritableStreamInterface $writableStream = null)
```
parameter $stream can be
- a resource (see php fopen)
- stream implementation either implementing ReadableStreamInterface or WritableStreamInterface or both
- a string. Will create a temporary (php://temp) stream containing the string
- null or empty. Will create an empty temporary (php://temp) stream
- a callback function which will be immediately called. The return value should be
an array containing [$stream, $options, $writableStream]

Optionally an $options array can be passed defining meta-data of the stream,
if information is available e.g. from prior operations

The stream constructor fails silently. I.e. any exceptions thrown during __construction will be catched, cached and
emitted as error events.

----

## __construct
creates an StreamInterface instance

```php
__construct($stream = '', array $options = array(), \React\Stream\WritableStreamInterface $writableStream = null)
```
parameter $stream can be
- a resource (see php fopen)
- stream implementation either implementing ReadableStreamInterface or WritableStreamInterface or both
- a string. Will create a temporary (php://temp) stream containing the string
- null or empty. Will create an empty temporary (php://temp) stream
- a callback function which will be immediately called. The return value should be
an array containing [$stream, $options, $writableStream]

Optionally an $options array can be passed defining meta-data of the stream,
if information is available e.g. from prior operations

The stream constructor fails silently. I.e. any exceptions thrown during __construction will be catched, cached and
emitted as error events.
