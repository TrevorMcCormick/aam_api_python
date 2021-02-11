# Adobe Audience Manager - Python Extension

This is a Python wrapper for the Adobe Audience Manager API.

To get started [Generate a JWT Authentication using Adobe IO](link)

This package requires you to create a .json document with the following credential details: client ID, client secret, tech account ID, tech account email, and organization ID. In a separate file, you also need generate a public/private key pair.

Once you have these documents, you can get install the package and login:

```sh
pip install aam-api
```

```py
adobe_aam_python.login('path/to/credentials.json', 'path/to/private.key')
```

Your authentication token should be tied to a Product Profile, which controls the actions you can execute and the objects on which you can act. If you are unable to perform an action supported by this package, the error is likely due to a permissions issue within the credentials setup.
