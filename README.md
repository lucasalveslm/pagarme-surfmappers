# Pagarme Surfmappers
An simple implementation of Pagar.me API to be used by Surfmappers.com

# Install
```Todo```

# How to use
You can use this lib as Pagar.me documentation suggests to. Above we'll show some examples

## Transaction
You can create an transaction.

```python
import pagarme_surfmappers

params = {...}  # As in Pagar.me documentation

pagarme_surfmappers.set_api_key(YOUR_API_KEY)
transaction = pagarme_surfmappers.Transaction()
response = transaction.create(params)

print(response)
```

## Capture Transcation
After create an transaction, you can capture it.

```python
import pagarme_surfmappers

params = {...}  # As in Pagar.me documentation

pagarme_surfmappers.set_api_key(YOUR_API_KEY)
transaction = pagarme_surfmappers.Transaction()
response = transaction.capture(params)

print(response)
```

## Recipient
Creates a recipient

```python
import pagarme_surfmappers

params = {...}  # As in Pagar.me documentation

pagarme_surfmappers.set_api_key(YOUR_API_KEY)
recipient = pagarme_surfmappers.Recipient()
response = recipient.create(params)

print(response)
```

## Recipient's Balance
You can also get an recipient's balance

```python
import pagarme_surfmappers

recipient_id = 'SOME_ID'

pagarme_surfmappers.set_api_key(YOUR_API_KEY)
recipient = pagarme_surfmappers.Recipient()
response = recipient.get_balance(recipient_id)

print(response)
```

# Contributing
The main purpose of this repository is to continue to evolve Pagar.me api code, making it faster and easier to use. Development of React happens in the open on GitHub, and we are grateful to the community for contributing bugfixes and improvements. Read below to learn how you can take part in improving React.

# License
This lib is [MIT licensed](./LICENSE).