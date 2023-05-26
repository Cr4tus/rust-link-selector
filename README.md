# Rust Link Selector

## What does the app do?
Displays all the links present in a webpage (a HTML document which comes from https://www.rust-lang.org).

## Programming Languages:
- Rust

## Frameworks & Libraries:
- error-chain - https://crates.io/crates/error-chain | https://docs.rs/error-chain/latest/error_chain/
- reqwest - https://docs.rs/error-chain/latest/error_chain/ | https://docs.rs/reqwest/latest/reqwest/
- select - https://crates.io/crates/select | https://docs.rs/select/0.6.0/select/
- tokio - https://tokio.rs | https://docs.rs/tokio/latest/tokio/

## Implementation:
First of all, lets mention how the errors are being handled: with the **error-chain** Rust library. The rest is pretty straight forward, the program makes a *GET* request to a website and prints the value of the *href* attribute present on **<a/\>** type HTML elements.