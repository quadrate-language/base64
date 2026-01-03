# base64

Base64 encoding and decoding for Quadrate.

## Installation

```bash
quadpm install https://github.com/quadrate-language/base64
```

## Usage

```qd
use base64

fn main() {
    // Encode to base64
    "Hello" base64::encode -> encoded
    encoded print nl  // "SGVsbG8="

    // Decode from base64
    "SGVsbG8=" base64::decode -> decoded
    decoded print nl  // "Hello"
}
```

## API

### Functions

- `encode(input:str -- encoded:str)` - Encode string to base64
- `decode(encoded:str -- decoded:str)` - Decode base64 string

## License

MIT
