# Friendsite List "API"
A basic JSON list of websites of a group of friends, TCP.

# Current Members On list
- Anjelo - https://www.anjelogo.com
- Evan - https://www.evanoctave.dev
- Patrick - https://projectpatatoe.pt23.net
- Caden - https://www.cadensantiago.com

# JSON Scheme
The JSON file just has 2 properties required. Whether you add an additional property, is wholly dependent on the receiving client to use that data.

The required schema is as follows:
```
[
  {
    "displayName": string,
    "url": string,
  }
]
```

## URL Formatting
URLs should append `http/https` with clients handling normalization and redirects. These URLs should point to the "main" or "landing" page of the individual.

## Additional Properties
As stated earlier, any additional properties are dependent on clients. For instance, if a client wanted to render special effects for individual sites, one would append `"effects": "sparkly"` or if individuals wanted to have special formatting, something like `"formatting": ["strong", "italicized"]`. Again, these properties are rendered via individual clients, and are not required to be implemented.
