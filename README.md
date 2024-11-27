## X Financial Technologies

USDX is the first SEC-regulated yield-bearing stablecoin for the United States.



Pricing
About
Sign in
Open account
Business banking for the digital age
A modern banking platform, powered by stablecoins and backed by U.S. Treasuries, to make global finance faster, seamless, and secure.
Contact sales
Open account
Dakota is a financial technology company, not a bank. Banking services are provided through global bank partners. U.S. partners are FDIC members.
Secure banking dashboard
Trusted by
logo
logo
logo
logo
logo
logo
/
Get global access to U.S. dollars
Dakota makes it easy for you to access banking services anywhere in the world.
Accept and send USD globally
Transfer USD quickly with ACH, Fedwire, SWIFT, and SEPA so your business can operate globally with ease.
Deposits held as U.S. Treasuries
Earn up to 4% rewards
Corporate cards with controls
Use stablecoins for 24/7 transfers
Reporting and automation
Payments screen in appPayments screen in appDeposits held as U.S. TreasuriesExample of yield growth over timeReports screen in appPermissions screen in appAccounting demonstration
Every dollar backed by U.S. Treasuries
Optimized Operations
Streamline your workflows and operate globally.
Operations account screen in app
Faster Global Payments
Move money faster with a smart transaction router that selects the best banking partner for each transfer.
Simplified Multi-Currency Accounts
Accept and send USD, EUR, and more (local currencies coming soon) with seamless account management.
Automated Accounting Made Easy
Save time with automated accounting tools and advanced reporting to keep your finances in sync.
Maximize Returns, Minimize Risk
Earn up to 4% rewards on your entire balance.
Tailored Yield Options
Earn yield aligned to your risk tolerance, from conservative to growth-focused.
Secure Asset Control
Retain full control of your U.S. Treasury-backed assets, safeguarded from bank failures and institutional risks.
Comprehensive Treasury Tools
Manage crypto, tokenized real-world assets, treasuries, and bonds in one seamless platform.
Treasury account screen in app
Business Leaders
Secure, manage, and grow your business, all in one place.
Dashboard screen in app
360-view of your treasury
See your entire financial picture in one place by connecting your bank accounts and wallets.
Maintain ownership
Keep control of your assets. They’re never at risk of default on a bank’s balance sheet.
Enterprise security and controls
Set detailed user controls for all levels of account holders with a customizable policy engine.
Bank with confidence, without the bank.
Industry-leading security
Industry-leading security
Protect your account with hardware-backed authentication, custom security policies, and 3rd-party security audits.
Built-in compliance
Built-in compliance
Integrated transaction monitoring tools score transactions and automate compliance checks.
Insurance
Insurance
Deposits and balances are protected by top insurance plans. Hold broad coverage to ensure your assets are safe.
24-7 support
24-7 support
Whenever, wherever you need help, our support channels are standing by. Find us on Slack and know we’ll be there to take care of you.
Frequently asked questions
Can I replace my traditional bank with Dakota?
Yes. With Dakota, you can seamlessly send and receive US dollars just like a traditional bank account. However, behind the scenes, your transactions are smarter and safer. Every dollar you deposit is automatically converted into stablecoins, which are then backed by US treasuries in our secure digital environment.
Can I use Dakota along with my existing bank?
Is Dakota a bank?
How is my money protected with Dakota?
What exactly are stablecoins?
What does "non-custodial" mean at Dakota?
Experience
Our team has built products that custody $100B in crypto and worked at the leading fintech and security companies.
logo
logo
logo
logo
logo
A new type of account, one without the banks.
Starting and operating a business is hard. Obstacles separate us from our goals. Some of them can’t be helped. Others exist because a select few rig the rules in their favor. 
We created Dakota because traditional banking has been one of those obstacles. It takes days to move your money. It pays tenths of a penny on the dollar. It will refuse your business on a whim. When it crashes, it gets the bailout and you are caught holding the bag. It’s the ultimate insider’s club that’s been fraught with fraud and you end up paying the price.
Dakota is a new type of account, one without the banks.
We leverage stablecoins, backed by US treasuries, to offer a global business account — available immediately to countless countries, and endless business partners, enabling seamless cross-border transactions, and access to an unmatched yield that puts you firmly in control of your finances.
How it works
Make USD transactions by ACH or wire transfer, without a traditional bank account. Deposits are converted to stablecoins and backed by U.S. Treasuries for added security and flexibility.

https://github.com/dakota-xyz/recovery

Recovery tool
This recovery tool can be used by Dakota customers to recover their keys. It requires a decrypted backup shard, the client shard, and a JSON file with the key mappings.

The format of the key mappings JSON file should be similar to

{
  "organization_id": "e65ccfaa-01b7-4a00-aec5-0fcc25d7eba7",
  "keys": [
    {
      "address_sub_id": "21d3969c-8a56-46d9-be38-b53c21294e54",
      "network_id": "solana-mainnet",
      "curve": "ELLIPTIC_CURVE_ED25519"
    },
    {
      "address_sub_id": "a09d020a-1bc8-47b6-a208-0fd47cd05e66",
      "network_id": "ethereum-mainnet",
      "curve": "ELLIPTIC_CURVE_SECP256K1"
    }
  ]
}
Build
Install Go 1.21 or higher:
Currently, recovery uses Go 1.21 to compile the code.

Install Go 1.21 by following instructions there, e.g.:

wget https://go.dev/dl/go1.21.3.linux-amd64.tar.gz
sudo tar xzvf go1.21.3.linux-amd64.tar.gz -C /usr/local/
export PATH=$PATH:/usr/local/go/bin
Verify the installation by typing go version in your terminal.

$ go version
go version go1.21.3 darwin/amd64
Build Recovery
In order to build recovery you need the source code. Either download the source of a release or clone the git repository.

Build recovery from the source code:

cd recovery
make build
After building, you should see a new executable file recovery/build/recovery.

Example usage
$ ./recovery -h
Usage of ./recovery:
  -keymap string
        Location of the JSON file containing the key map
  -shard1 string
        Location of the file containing the first shard
  -shard2 string
        Location of the file containing the second shard
  -target string
        Target CSV file (default "keys.csv")
$ ./recovery -shard1 shard1.bin -shard2 shard2.bin -keymap backup.json
2023/11/09 03:20:10 INFO Initiating recovery
2023/11/09 03:20:10 INFO Recovery complete. Results saved to keys.csv
$ cat keys.csv
Network,Address,PrivateKey
solana-mainnet,4tZpnxbJbkCDFFCpbmb4y7wsH366kxeb57R8owi67qi8,2tFuN9PCkTYsDV6rq8RauJZEmyBs7x8rLoSAFYD5JcQMCzVzStq45VeUVDDghGqXaYm8muC8YECzgoqTkyPph8gp
ethereum-mainnet,0x0D7ad5799E3DB77c8258b9700E4f94Fcb092C64B,0x222d55b028c7896058d28af1d44c55d45264c470f2a93e7b013076e68b7bfa25
