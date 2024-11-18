# License.pay - Monetize Your Github

[**License.pay**](https://licence-pay-app.vercel.app/) is a licensing format that enables monetization of open-source software strictly for AI usage. It allows developers to set clear terms for code usage by AI while ensuring fair compensation.

## Three Simple Steps

1. **Use OpenCommerce SDK**  
   Integrate our SDK to open an account and start receiving payments from AI agents.

2. **Create LICENSE.pay**  
   Use our [wizard](https://licence-pay-app.vercel.app/) to generate your custom license file.

3. **Add to GitHub**  
   Place LICENSE.pay in your repository root.

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
- Use the funding widget:
```python
sdk.prompt_funding()
```
- Or send funds directly to your account address using your preferred wallet


## License

This project is licensed under the MIT License.

## Support

- Open an issue on GitHub
- Contact: idan@opencommerce.xyz
