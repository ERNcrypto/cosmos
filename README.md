# cosmos
# autodelegate_nibiru

### Install screen
    apt-get install screen
    curl -s https://raw.githubusercontent.com/ERNcrypto/cosmos/main/prepare-nodejs.sh | bash
### Install NodeJs
    curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
    sudo apt-get install -y nodejs
### Install shelljs --cli
    npm install shelljs --cli
### Download script
    cd && wget -O autodelegate_nibiru.js https://raw.githubusercontent.com/ERNcrypto/cosmos/main/autodelegate_nibiru.js
### Edit the file
    nano ~/autodelegate_nibiru.js

### Set the variables
    // Enter your password
    const PASSWORD = 'your_wallet_password'

    // Enter your valoper address
    const VALOPER = 'nibivaloper.........'

    // Enter your wallet address
    const DELEGATOR = 'nibiru_wallet_address'

    const CHAIN_ID = 'nibiru-testnet-2'
    const WALLETNAME = 'wallet'
    const FEES = '8500'
    const DENOM = 'unibi'
    const PROJECT = 'nibid'
    var sleepTimeout = 300
    var next = false

    // Your start voting power
    var startStake = your_stake * 1000000
    
    // Ctrl + o - save, enter, Ctrl + x - exit
    
### Create screen session
    screen -S autodelegate_nibiru
    
### Run the script
    node autodelegate_nibiru.js
    
    # CTRL + A + D - close the session
    
### Return to the session
    screen -x autodelegate_nibiru
