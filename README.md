ctail
=====

`ctail` is a small configurable Bash script which can colour log entries outputted through `tail`. It actually wraps `tail`, piping its
output through an `awk` script that colorizes the output according to log severity levels.

### Overriding default log levels and colors
A `ctail.config` file can be used to configure `ctail` in order to use different colours for various log levels. The file must be in the
same folder as `ctail`. For an example file, please check the `ctail.config` file from the repository.

### Compatibility with Mac OS X
Should work on Mac OS X without any modification.
