# Wordlist
allchain Brain Wallets wordlist library


[Rust Documentation](https://docs.rs/allchain-wordlist/)


# RUST

```toml
# Cargo.toml

[dependencies]
allchain-wordlist = "1.2"
```

```rust
# main.rs

extern crate allchain_wordlist;

fn main() {
  println!("Words: {}", allchain_wordlist::random_phrase(12));

  let phrase = "violin oblivion cylinder list disarray wobbly fastball showplace oasis patronize septic spearhead";
  println!("Valid: {:?}", allchain_wordlist::validate_phrase(phrase, 12));
}
```


# JavaScript


```bash
$ npm i @allchain/wordlist --save
```


```js
// main.js

import { randomPhrase, verifyPhrase } from '@allchain/wordlist'

console.log(randomPhrase(12))

// This will throw if the phrase is not valid:
verifyPhrase("violin oblivion cylinder list disarray wobbly fastball showplace oasis patronize septic spearhead", 12)
```

