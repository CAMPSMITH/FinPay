# FinPay

FinPay is an enhancement to Fintech Finder that enables customers to instantly pay the fintech professionals whom they hire with cryptocurrency.

---

## Technologies

* **Web3.py** - A Python library for connecting to and performing operations on Ethereum-based blockchains.

* **ethereum-tester** - A Python Library that provides tools for testing Ethereum-based applications.

* **mnemonic** - A Python Library for generating a 12- or 24-word mnemonic seed phrase based on the BIP-39 standard.

* **bip44** - A Python Library for deriving hierarchical deterministic wallets from a seed phrase based on the BIP-44 standard.

* **Ganache** - Utility that simplifies and faclitates local blockchain development and testing.

* **Streamlit** - A Python library used to create shareable web applications from python programs.

---

## Installation Guide

### Install required dependencies

```
pip install web3==5.17
pip install eth-tester==0.5.0b3
pip install mnemonic
pip install bip44
```

### Install Ganache

For instructions on installing Ganache in your local environment, follow the directions in the [Ganache Download Page](https://www.trufflesuite.com/ganache).

### Install Streamlit
If streamlit is not installed in your vm, install it with
```
conda install streamlit
```

---

## Usage

1. Start Ganache Quickstart.
2. Copy the **mnemonic** from Ganache and store it in a **.env** file as shown below

    .env
    ```
    MNEMONIC="<the mnemonic phrase from Ganache>"
    ```

3. start the application

    ```
    streamlit src/fintech_finder.py
    ```
    
---

## Demo



https://user-images.githubusercontent.com/9788128/180631388-763e1d35-609d-4197-bec4-066c8be272f8.mov



### Selecting a FinTech Professional
The following screenshot shows how a Fintech professional is selected and how the hours for the job are inputted.  Notice that the wage is calculated. 
![select fintech professional](/images/finpay_select_professional.png)

### Pay FinTech Professional
After the Fintech professional is selected and hours are inputted, the payment transaction can be executed by pressing the **Send Transaction**  button.  Notice that the transaction hash is shown after the tansaction is submitted.
![pay fintech professional](/images/finpay_pay_professional.png)

### Payment Transaction
The payment transaction can be viewed from the Ganache Transaction screen.
![payment transaction](/images/finpay_transaction.png)

### Sender Account Balance/History
The sender's account balance is decremented by the amount of the transaction.  The number of transaction this sender has sent is shown on the right.
![sender balance](/images/finpay_sender_balance.png)

### Receiver Account Balance/History
The receiver's account balance is incremented by the amount of the transaction.  The number of transaction this receiver has sent is shown on the right.
![receiver balance](/images/finpay_receiver_balance.png)

---

## Contributors

*  **Martin Smith** <span>&nbsp;&nbsp;</span> |
<span>&nbsp;&nbsp;</span> *email:* msmith92663@gmail.com <span>&nbsp;&nbsp;</span>|
<span>&nbsp;&nbsp;</span> [<img src="images/LI-In-Bug.png" alt="in" width="20"/>](https://www.linkedin.com/in/smithmartinp/)


---

## License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
