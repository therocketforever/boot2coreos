
# Boot2coreos

Like boot2docker but with CoreOS.

## Features

- Run docker directly from your mac 
- Access all ports via private ip `13.0.3.3` with no port mapping required.
- Persistent file storage
- Leverage all of the features from [CoreOS](https://coreos.com)

## Requirements

- [Vagrant](http://www.vagrantup.com) must already be installed
- [Docker](http://docker.io) must be installed if you wish to run docker commands from your mac

## Installation

### Clone boot2coreos from github

```
$ git clone https://github.com/Bodhi5/boot2coreos.git
```

### start boot2coreos

From the boot2coreos directory run

```
$ vagrant up
```

### Set the environment variable for the docker daemon

```
$ export DOCKER_HOST=tcp://13.0.3.3:4243
```

## Advanced usage

### Port forwarding / folder sharing

These can be enabled via the Vagrant file. After updating the Vagrant file run a `$ vagrant reload` and they should be applied.

### SSH into VM

To ssh in to the machine you must be in the directory that contains the `Vagrantfile`

```
$ vagrant ssh
```

## License

  The MIT License (MIT)

  Copyright (c) 2014 <Bodhi5, Inc>

  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:

  The above copyright notice and this permission notice shall be included in
  all copies or substantial portions of the Software.

  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  THE SOFTWARE.
