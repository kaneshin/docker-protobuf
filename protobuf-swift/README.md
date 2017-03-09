# Protocol Buffer for Swift on Docker

[![Docker Stars](https://img.shields.io/docker/stars/kaneshin/protobuf-swift.svg)](https://hub.docker.com/r/kaneshin/protobuf-swift/)
[![Docker Pulls](https://img.shields.io/docker/pulls/kaneshin/protobuf-swift.svg)](https://hub.docker.com/r/kaneshin/protobuf-swift/)
[![Docker Automated buil](https://img.shields.io/docker/automated/kaneshin/protobuf-swift.svg)](https://hub.docker.com/r/kaneshin/protobuf-swift/)

## Usage


    # print help message of protoc
    docker run -it --rm kaneshin/protobuf-swift --help

    # execute to output files.
    docker run -it --rm -v $PWD:/proto:rw kaneshin/protobuf-swift --swift_out=. *.proto

    # execute to output files by user.
    docker run -it --rm -v $PWD:/proto:rw kaneshin/protobuf-swift -u $(id -u):$(id -g) --swift_out=. *.proto

## License

[The MIT License (MIT)](http://kaneshin.mit-license.org/)

## Author

Shintaro Kaneko <kaneshin0120@gmail.com>
