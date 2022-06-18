# vault 1.10.4

Start : 
```
docker-compose up
```
Stop :
```
docker-compose down
```

---

## First start Vault

http://localhost:8200/ui

![img data](/images/vault_1.png?raw=true "img Data title")

Key shares
```
5
```
Key threshold
```
3
```

click -> Initialize

Vault has been initialized! Here are your 5 keys.

![img data](/images/vault_2.png?raw=true "img Data title")

Download keys

file - > vault-cluster-vault-2022-06-18T11_01_19.177Z.json
```json
{
  "keys": [
    "06eb3120fd83b0ee982406e2f8f37aa0cf79e4e931582f2c1fd4a0154bd729e5e4",
    "a55303f0660baa59a280a0b619eda187d0f70397b02e5b3bfcf55a09d877de4f89",
    "f6eefbe65ec5d6d177b642e166c6df0bbb1ad41eef0517d4f059b7621db64a972b",
    "93f929110666be22cdcd6734a14b0b9c9b142fafa8595ca7646c9543903e1c64e5",
    "fdec818d2af9615c57c35e7da3655661148afcd61642e1e676f0f547cb06a646d1"
  ],
  "keys_base64": [
    "BusxIP2DsO6YJAbi+PN6oM955OkxWC8sH9SgFUvXKeXk",
    "pVMD8GYLqlmigKC2Ge2hh9D3A5ewLls7/PVaCdh33k+J",
    "9u775l7F1tF3tkLhZsbfC7sa1B7vBRfU8Fm3Yh22Spcr",
    "k/kpEQZmviLNzWc0oUsLnJsUL6+oWVynZGyVQ5A+HGTl",
    "/eyBjSr5YVxXw159o2VWYRSK/NYWQuHmdvD1R8sGpkbR"
  ],
  "root_token": "hvs.Ba1s0wTIlTTQUER0Fabhtrx8"
}
```
Click -> Continue to Unseal

Unseal Vault

![img data](/images/vault_3.png?raw=true "img Data title")

keys_base64 from vault-cluster-vault-2022-06-18T11_01_19.177Z.json

Row 1 -> BusxIP2DsO6YJAbi+PN6oM955OkxWC8sH9SgFUvXKeXk

Click -> Unseal

![img data](/images/vault_4.png?raw=true "img Data title")

Row 2 -> pVMD8GYLqlmigKC2Ge2hh9D3A5ewLls7/PVaCdh33k+J

Click -> Unseal

![img data](/images/vault_5.png?raw=true "img Data title")

Row 3 -> 9u775l7F1tF3tkLhZsbfC7sa1B7vBRfU8Fm3Yh22Spcr

Click -> Unseal

![img data](/images/vault_6.png?raw=true "img Data title")

root_token -> hvs.Ba1s0wTIlTTQUER0Fabhtrx8

Click -> Sign in

![img data](/images/vault_7.png?raw=true "img Data title")

---