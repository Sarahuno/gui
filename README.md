
## Overview

This project uses Loadstring hosting to serve `.lua` files. The hosting service allows you to use `https://gui.rf.gd` as a domain to access and execute `.lua` scripts.

## How It Works

### Using the Loadstring Host

To use the Loadstring host with your `.lua` file, follow these steps:

1. **Host Your `.lua` File:**
   - Ensure that your `.lua` file is committed to your repository.

2. **Access the File via URL:**
   - Construct the URL to access your `.lua` file using the following format:
     ```
     https://gui.rf.gd?s=FileName.lua
     ```

3. **Use the URL in Loadstring:**
   - Use the URL in a `loadstring` function to execute your script:
     ```lua
     loadstring("https://gui.rf.gd?s=FileName.lua")()
     ```

### Example

If you have a file named `example.lua`, you would use:
```lua
loadstring("https://gui.rf.gd?s=example.lua")()
