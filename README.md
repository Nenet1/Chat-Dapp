Contract Address: 0x69865e77e5f8238c094C2dC1646C87f8E3bc1Db3

## Ethereum Name Service (ENS) Contract
### Overview
This Ethereum smart contract provides a basic implementation of a name service system, similar in spirit to the Ethereum Name Service. It allows users to register a unique name along with an image URI to an Ethereum address. Each Ethereum address can only be associated with one name, and each name can only be registered to one address.

### Features
Register a Name: Users can register a unique name to their Ethereum address.
Retrieve Profiles: Users can retrieve profile information by name or Ethereum address.
List All Profiles: Fetch a list of all registered profiles.
Errors
NAME_ALREADY_EXISTED: Thrown if the name is already registered.
ADDRESS_ALREADY_REGISTERED: Thrown if the Ethereum address is already associated with a name.
NAME_NOT_YET_REGISTERED: Thrown if the name has not been registered yet.
ADDRESS_NOT_YET_REGISTERED: Thrown if the Ethereum address has not been registered yet.


### Chat Contract
### Overview
The Chat contract provides a decentralized chat system integrated with an Ethereum Name Service (ENS). It allows users to send messages to each other using their ENS registered names instead of directly using Ethereum addresses. The contract ensures that messages can only be sent to valid registered ENS names, leveraging an ENS contract interface for name resolution.

### Features
Send Messages: Users can send messages to each other using ENS names.
Retrieve Messages: Users can retrieve their chat history with a specific ENS name.
Integration with ENS: Utilizes an ENS contract to resolve names to Ethereum addresses and vice versa.
Errors
RECEIVER_DOES_NOT_EXIST: Thrown if the receiver's ENS name does not resolve to a valid Ethereum address.
