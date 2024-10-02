# CDN Tokens

For both musiclibrary and sfxlibrary, there are 2 optional parameters that are sent by the GD client but are currently **not** required to receive the data. One still may want to implement these into their code for future-proofing.

#### `expires`

This is the UNIX timestamp (seconds) that is an hour later than the current timestamp.

#### `token`

Tokens are generated this way (pseudocode):

```
# The endpoint is the part of the URL after https://geometrydashfiles.b-cdn.net. So, for example, the endpoint for https://geometrydashfiles.b-cdn.net/sfx/sfxlibrary_version.txt would be /sfx/sfxlibrary_version.txt
hash = md5("8501f9c2-75ba-4230-8188-51037c4da102{endpoint}{expires}")
base64EncodeUrlSafe(hash.digest(ASCII))
```

Please note that the hash must be digested as ASCII, not hexadecimal!
