# Define the target object file for the kernel module
obj-m += hello-1.o

# Use the current working directory
PWD := $(shell pwd)

# Build the kernel module
all:
	$(MAKE) -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

# Clean up build files
clean:
	$(MAKE) -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
