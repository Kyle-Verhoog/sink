[![Build Status](https://travis-ci.org/Kyle-Verhoog/sink.svg)](https://travis-ci.org/kyle-verhoog/sink) [![Gitter](https://badges.gitter.im/Kyle-Verhoog/sink.svg)](https://gitter.im/Kyle-Verhoog/sink?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

# sink
sink things

access your dropbox from the comforts of your terminal

## Install

```sh
  $ git clone https://github.com/kyle-verhoog/sink && cd sink
  $ python setup.py
  $ export PATH=/path/to/sink/sink.py/:$PATH
```

Hopefully in the future...

```sh
  $ pip install sink
```

## Usage

Examples

```sh
  $ # Upload some taytay to dropbox
  $ cd music/taylor swift/singles
  $ sink cd music/taytay
  $ sink up bad_blood.mp3
```

```sh
  $ # Share your spacemacs configuration
  $ cd
  $ sink share .spacemacs
```
  
## Development

### Code Formatting

Style: see https://www.python.org/dev/peps/pep-0008

Formatter: Google's [YAPF](https://github.com/google/yapf)

```sh
  $ pip install yapf
```

Usage

```sh
  $ # Apply the formatter to a file in-place (-i)
  $ yapf -i --style="pep8" <file.py>
```

### Tokens
In order to use the Dropbox API you need an OAuth2 token to be generated for your dropbox account. You can generate one for development by creating an app and generating an access token.
