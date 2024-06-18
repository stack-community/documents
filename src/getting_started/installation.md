# Installation

Paste below shell script on the your terminal.
It installed Stack develop environments.

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
git clone https://github.com/stack-community/stack-lang.git
cargo install --path ./stack-lang
```

It's sucessful installation! if you enter `stack` and `stack-server` on the your shell then displayed REPL.
> REPL is stand for read-eval-print loop. It's usual way in many language's intterpreter.