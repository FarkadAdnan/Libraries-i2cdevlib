# Libraries-i2cdevlib
All libraries for equilibrium
I2C Device Library Kit for Arduino or other C++ based MCUs

- The I2C Device Library (i2cdevlib) is a collection of mostly uniform and well-documented classes to provide simple and intuitive interfaces to I2C devices. Each device is built to make use of the generic "I2Cdev" class, which abstracts the I2C bit- and byte-level communication away from each specific device class, making it easy to keep the device class clean while providing a simple way to modify just one class to port the I2C communication code onto different platforms (Arduino, PIC, MSP430, Jennic, simple bit-banging, etc.). Device classes are designed to provide complete coverage of all functionality described by each device's documentation, plus any generic convenience functions that are helpful.

- There are examples in many of the classes that demonstrate basic usage patterns. The I2Cdev class is built to be used statically, reducing the memory requirement if you have multiple I2C devices in your project. Only one instance of the I2Cdev class is required. Recent additions as of late 2021 have also made it possible to pass in non-default Wire objects (in the Arduino environment) to allow using multiple I2C transceivers at the same time, specifically because of the number of people who wanted to use up to four MPU-6050 IMUs without I2C mux ICs involved.

- Documentation for each class is created using Doxygen-style comments placed in each class definition file, based on the information available in each device's datasheet. This documentation is available in HTML format on the i2cdevlib.com website, which also holds helpful information for most of the classes present here on the repository.
