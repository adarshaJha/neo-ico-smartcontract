<p align="center">
  <img
    src="https://assets.brandfolder.com/p429iy-cjzaz4-epdy6e/v/1550884/view.png"
    width="125px;">
</p>
<h3 align="center">Thor ICO Smart Contract</h3>
<p align="center">Thor Token Offical ICO Smart Contract.</p>
<p align="center">Based of Neo ICO Template by NEX team - https://github.com/neonexchange/neo-ico-template</p>
<hr/>

#### Requirements

Usage requires Python 3.6+

#### Installation

Clone the repository and navigate into the project directory. 
Make a Python 3 virtual environment and activate it via

```shell
python3 -m venv venv
source venv/bin/activate
```

or to explicitly install Python 3.6 via

```shell
    virtualenv -p /usr/local/bin/python3.6 venv
    source venv/bin/activate
```

Then install the requirements via

```shell
pip install -r requirements.txt
```

#### Compilation

The template may be compiled as follows

```python
python3 compile.py
```


This will compile your template to `ico_smart_contract.avm`

#### Import

In neo-python prompt:

```neo-python
import contract path_to/neo-ico-smartcontract/ico_smart_contract.avm 070202 02 True True
```

#### Deploy (Owner Check)

In neo-python prompt:

```neo-python
testinvoke 0xd95fd65c6019b63ff6c9a8d7a26ff5171e57b69f deploy []
```

#### Register KYC (Owner Check)

In neo-python prompt:

```neo-python
testinvoke 0xd95fd65c6019b63ff6c9a8d7a26ff5171e57b69f crowdsale_register ['AK2nJJpJr6o664CWJKi1QRXjqeic2zRp8y']
testinvoke 0xd95fd65c6019b63ff6c9a8d7a26ff5171e57b69f crowdsale_status ['AK2nJJpJr6o664CWJKi1QRXjqeic2zRp8y']
```

#### Mint Token (KYC Check)

In neo-python prompt:

```neo-python
testinvoke 0xd95fd65c6019b63ff6c9a8d7a26ff5171e57b69f mintTokens [] --attach-neo=1
```

#### Airdrop - For privatesale (Owner Check)

In neo-python prompt:

```neo-python
testinvoke 0xd95fd65c6019b63ff6c9a8d7a26ff5171e57b69f airdrop ['AaYZVFjjxae4tiXjCepwp7tEAhn4SwF9Nu', 1000]
```

#### Current Status: In Progress

Thor Token engineering team is actively working on the smart contract for both of the upcoming pre-sale & crowd-sale. More information regarding the KYC and Whitelist process will be annouced soon. Please join our Telegram to get the most up to date information about our progress. https://t.me/joinchat/F-UKj1Md5AilZgV9zU0Dwg