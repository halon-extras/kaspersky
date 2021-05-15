## kaspersky_av(fp[, options])

Scan a File pointer (fp) with Kaspersky Anti-virus (using HTTP POST). This function should be used with the [`per_message` cache](http://docs.halon.se/hsl/structures.html#cache).

**Params**

- fp `File` - the mail file
- options `array` - options array

**Returns**: an array with ``scanResult`` and optionally ``detectionName`` (see Kaspersky documentation), None on error.

The following options are available in the **options** array.

- timeout `number` - Timeout in seconds. The default is 2 seconds.
- host `string` - IP-address of the kavhttpd server. The default is `127.0.0.1`
- port `number` - TCP port. The default is `80`
