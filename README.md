# shiver
A cold wallet for Nano.

## To-Do
  1. ``0/5`` Transfer instructions and text over to new UI.
  2. ``4/5`` Add client side validation.
  3. ``3/5`` Create Wizard.

## Wizard

Information
  - What is your Nanode API key?
  - Action:
    - Open an account.
    - Receive Nano.
    - Send Nano.
    - Change your representative.
      
  1. Open
    - What is the transaction hash? Maybe Nano Faucet.
    - What would you like your representative to be?
      - Account: Linked account
      - Previous: 0
      - Representative: Representative
      - Balance: Amount sent (use extra info api call).
      - Link: Hash
  2. Open Sign
    -  Here is your hash: What is your signature?
      - Work: 0000000000000000
      - Signature: Signature
  3. Results:
    - Block processed.
    - Here is your hash:
    
  1. Receive
    - What is the transaction hash?
      - Account: Linked account
    - Grab Account details
      - Previous: Frontier
      - Representative: Representative
      - Balance: Amount sent (use extra info api call) + current balance.
      - Link: Hash
  2. Receive Sign
    -  Here is your hash: What is your signature?
      - Work: Generate work
      - Signature: Signature
  3. Results:
    - Block processed.
    - Here is your hash:
    
  1. Send
    - What is your Account?
      - Account: Account
    - Grab Account details
      - Previous: Frontier
      - Representative: Representative
    - what is the amount?
      - Balance: current balance - amount sent (use extra info api call).
    - What is the destination address?
      - Link: Hash
  2. Send Sign
    -  Here is your hash: What is your signature?
      - Work: Generate work
      - Signature: Signature
  3. Results:
    - Block processed.
    - Here is your hash:
    
  1. Change
    - What is your account?
      - Account: Account
    - Grab Account details
      - Previous: Frontier
    - What is your representative?
      - Representative: Representative
      - Balance: current balance.
      - Link: 0000000000000000000000000000000000000000000000000000000000000000
  2. Change Sign
    -  Here is your hash: What is your signature?
      - Work: Generate work
      - Signature: Signature
  3. Results:
    - Block processed.
    - Here is your hash:

## Links

https://marvinroger.github.io/nanocurrency-js/index.html
https://github.com/nanocurrency/raiblocks/wiki/Universal-Blocks-Specification
