## Multi stage docker build

The reason to chose go is because it is a statistically type languae and there is now need for runtime. like pyhton, javascript which rely on
runtime to execute. go compiles directly to machine code, which then can be executed directly by the machine os.

So the advantage of multi stage build can be understand with the drastically decrease of image size.