# Tactility Tool

This is the build tool for building ESP32 applications.
It's uploaded to the CDN along with its content.

To use it, you only need the `tactility.py` script.
Run `python tactility.py --help` to show the options.

Applications are expected to have a `tactility.properties` file with content like this:

```properties
[sdk]
version = 0.4.0-dev
```

## Example usages

**Building all targets**

`python tactility.py build all`

**Building a specific target**

`python tactility.py build esp32s3`

**Testing the tool without building**

`python tactility.py build all --skip-build`

**Debugging issues**

Show more output:

`python tactility.py build all --verbose`

Remove temporary build files:

`python tactility.py clean`

Remove the SDK cache:

`python tactility.py clearcache`

## License

[MIT License](LICENSE.md)

