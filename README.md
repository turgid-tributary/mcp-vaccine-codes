# MCP Vaccine Code Server

Fetches the latest CDC vaccine code mapping and exposes tools to interact with it.

## Usage

```
npm i
npm run build
```

And then point to the `build/index.js` file in your MCP Client configuration.

I've tested this using Claude Desktop as my MCP Client with 

```json
{
  "mcpServers": {
    "vaccine-codes": {
      "command": "node",
      "args": [
        "/ABSOLUTE/PATH/TO/mcp-vaccine-codes/build/index.js"
      ]
    }
  }
}
```


## Example Queries

>What is the CVX code of anthrax?

```
I can help you find the CVX code for anthrax vaccine. Let me check the CVX vaccine database for you.

...

The CVX code for anthrax is 319.

Looking at the CVX vaccine database, the anthrax vaccine group (code 319) includes component vaccines with CVX codes 24, 318, and 319. The main anthrax vaccine group is designated as CVX code 319, which encompasses the various anthrax vaccine formulations available.
```





