# Ethereum_Payment_App
This is a proof of concept for an app that stores a directory of consultants and pays them with eth on the Ethereum blockchain.

## How to Use and Test the App with Ganache

[Ganache](https://trufflesuite.com/ganache/) is program that allows you to quickly set up a local blockchain, which you can use to test and develop smart contracts.

Ganache is a part of the Truffle Suite, which is a set of tools for developers who are using the Ethereum Virtual Machine. When you install Ganache, it creates an ephemeral blockchain that is stored on your local machine. This means that the blocks it creates are retired as soon as the purpose of recording the transaction is completed. This is ideal for testing purposes, because it means Ganache is both fast and lightweight.

### Send a test transaction by using the application’s web interface. Then look up the resulting transaction hash in Ganache to confirm that the completion of the transaction.

1. Make sure your development environment has access to the libraries listed in the Technologies section below.
2. Clone and Pull the github repository.
3. Store your Ethereum account mnemonic code for your test account in an .env file (ie. MNEMONIC = 'your mnemonic code').
4. From your terminal, navigate to the project folder that contains your `.env` file and the `fintech_finder.py` and `crypto_wallet.py` files.
5. To launch the Streamlit application, type `streamlit run fintech_finder.py`.

6. On the resulting webpage, select a candidate that you would like to hire from the appropriate drop-down menu. Then, enter the number of hours that you would like to hire them for. 
7. Click the Send Transaction button to sign and send the transaction with your Ethereum account information. If the transaction is successfully communicated to Ganache, validated, and added to a block, a resulting transaction hash code will be written to the Streamlit application sidebar.

8. Navigate to the Ganache accounts tab and locate your account (index 0).
![Ganache 4_11_2022 8_57_03 PM](https://user-images.githubusercontent.com/94941017/163826663-e944f88c-9fb7-4df6-8cbd-41d22b2bf564.png)

9. Navigate to the Ganache transactions tab and locate the transaction.
![Ganache 4_11_2022 8_58_03 PM](https://user-images.githubusercontent.com/94941017/163998035-ef36b3b1-15cc-4f43-ad0f-adf4001eea3a.png)

---

## Technologies

This application was written in python 3.7. It uses the following libraries:

* [bip44](https://pypi.org/project/bip44/) - For deriving hierarchical deterministic wallets from a seed phrase based on the BIP-44 standard.

* [web3](https://web3py.readthedocs.io/en/stable/overview.html) - For for connecting to and performing operations on Ethereum-based blockchains.

* [streamlit](https://github.com/voila-dashboards) - For publishing Jupyter notebook output as a web application.

---

## Contributors

Rachael Donham
rachaeldonham@gmail.com

---

## License

MIT
    
