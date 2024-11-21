# LICENCE.pay - Monetize Your Github

**Backgroundey**
AI is using more and more open-source code to train models and power applications, but the developers behind this code aren't getting paid for their work. It's a problem: AI companies are making money, but the creators of the code they rely on aren't seeing a share of that value. LICENCE.pay changes this by letting developers set clear terms for how their code can be used by AI, making sure they get compensated fairly without giving up the spirit of open source.

You can create a LICENCE.pay file, save it in your GitHub repository, and start getting fair compensation for your code. It’s simple to set up and ensures that your contributions are valued when used by AI systems for training or inference.

[**LICENCE.pay**](https://licence-pay-app.vercel.app/) is a licensing format that enables fair compensation for your open-source code, strictly for AI usage. 


## Three Simple Steps

1. **Use OpenCommerce SDK**  
   Integrate our SDK to open an account and start receiving payments from AI agents.

2. **Create LICENCE.pay**  
   Use our [wizard](https://licence-pay-app.vercel.app/) to generate your custom licence file.

3. **Add to GitHub**  
   Place LICENCE.pay in your repository root.


## Quick Start

1. **Install OpenCommerce SDK**
```bash
pip install opencommerce-sdk
```

2. **Initialize Your Account**
```python
from opencommerce_sdk import OpenCommerceAccountToolkit

# For production
sdk = OpenCommerceAccountToolkit(network='production')

# For testing
# sdk = OpenCommerceAccountToolkit(network='testnet')
```

3. **Get Your Account Address**
```python
account_address = sdk.get_account_address()
print(f"Your account is ready: {account_address}")
```

4. **Fund Your Account (You need ETH to send transactions and offramp)**
```python
sdk.prompt_funding()
```
- Or send funds directly to your account address using your preferred wallet/exchange.



## Licence

This project is licensed under the MIT Licence.


## Support

- Open an issue on GitHub
- Contact: idan@opencommerce.xyz
