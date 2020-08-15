# cardano-cli-bashrc
functions I use inside my `~/.bashrc` to manually sign transactions on air-gapped machine

Main functions create a `tx.raw` transactions and a raw terminal command (`cmd.txt`) that can be brought o the air gapped amchine for signing.

Once files have been signed you can bring the `tx.signed` file back to the on-line machine and submit it to the blockchain.
