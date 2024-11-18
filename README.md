# License.pay - Monetize Your Github

**License.pay** is a licensing format that enables monetization of open-source software strictly for AI usage. It allows developers to set clear terms for code usage by AI while ensuring fair compensation.

## Three Simple Steps

1. **Use OpenCommerce SDK**  
   Integrate our SDK to start receiving payments from AI agents

2. **Create LICENSE.pay**  
   Use our [wizard](https://licence-pay-app.vercel.app/) to generate your custom license file

3. **Add to GitHub**  
   Place LICENSE.pay in your repository root

## Quick Start

1. **Install OpenCommerce SDK**
```bash
pip install opencommerce-sdk
```

2. **Initialize Your Account**
```python
from opencommerce_sdk import OpenCommerceAccountToolkit

# For testing
sdk = OpenCommerceAccountToolkit(network='production')

# For testing
# sdk = OpenCommerceAccountToolkit(network='testnet')
```

3. **Get Your Account Address**
```python
account_address = sdk.get_account_address()
print(f"Your account is ready: {account_address}")
```

4. **Fund Your Account**
- Use the funding widget:
```python
sdk.prompt_funding()
```
- Or send funds directly to your account address using your preferred wallet

5. **Send Transactions**
```python
sdk.send_money(
    recipient_address='0xRecipientAddressHere',  # Address of the exchange or off-ramp
    amount_usdc=50.0  # Amount to transfer in USDC
)
```

## Implementation Steps

1. **Create Account**: Use OpenCommerce SDK to open an account for receiving and managing stablecoins
2. **Generate License**: Use our wizard to generate your custom LICENSE.pay file
3. **Deploy**: Place LICENSE.pay in your repository root

## License

This project is licensed under the MIT License.

## Support

- Open an issue on GitHub
- Contact: idan@opencommerce.xyz
