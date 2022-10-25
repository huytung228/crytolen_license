# CrytoLen License tutorial

## Register new account here
https://app.cryptolens.io/Account/Register

## Login to crytotolens
https://app.cryptolens.io/Account/Login

# Create new product
From `Product` section, select `Create new product`, fill all informations and, press `Create` \
![Alt text](images/create_product.png?raw=true "Optional Title")

# Get RSA Public Key and Access Token
Access [this](https://app.cryptolens.io/docs/api/v3/QuickStart), scroll to the bottom of the page, and get RSA Public Key and Access Token. Something look like this 
![Alt text](images/credential.png?raw=true "Optional Title")

# Get product id
From [products](https://app.cryptolens.io/Product) select product just created and get `Product Id`

# Create new license key
From product detail page, select `Create a new key` and fill information for `Set Time (in days)` and `Maximum number of machines` and select Create

# Activate License ai client side
From steps above we have:
- RSA pub key
- Access token
- Product ID
- License Key

Create environment file `.env` with these infomations. Example [here](.env)

To integrate license module into AI docker, add option `--env-file {path_to_env_file}` when run docker