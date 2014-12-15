# How to Recompile (Linux)

```
# Make modifications to .lua files in /src
vim /src/main.lua

# Zip up game files into a Love archive
cd src/
zip -9 -q -r ../02.love .

# Create 64-bit Windows executable
cat platforms/win64/love.exe 02.love > build/win64/02.exe

# Copy over DLLs and license
cp platforms/win64/*.dll build/win64/
cp platforms/win64/license.txt build/win64/
```
