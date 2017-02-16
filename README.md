
#CryptoAuthentication OpenSSL Engine  

##Overview
This is an OpenSSL Engine implementation using ATECC508A for ECC key storage, ECDSA sign/verify, ECDH, and FIPS Random Number Generator

The implementation integrates the [Microchip ATECC508A](http://www.microchip.com/wwwproducts/en/ATECC508A) into the [OpenSSL ENGINE API](https://www.openssl.org/docs/man1.0.2/crypto/engine.html) to provide secure hardware key storage, [CAVP certified random numbers](http://csrc.nist.gov/groups/STM/cavp/documents/aes/aesval.html), P256 ECDSA & ECDH, and secure storage for data.

This project will integrate the key creation and import capabilities of the ATECC508A into the OpenSSL key creation and certificate creation process. 

Also, secure key storage for RSA keys are implemented using the encrypted read/write feature of the ATECC508A. 

###Supported Cipher Suites
Many ECDH(E)-ECDSA and ECDHE-RSA cipher suites are supported with the OpenSSL Engine for ATECC508A implementation.  

Details for cipher suites can be found [here](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/Supported-Ciphers)

##Download and Make 
Build instructions for Linux can be found on the Wiki pages associate with this project.

See: [Compile OpenSSL Engine for ATECC508A on Linux](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/Linux:-Compile-OpenSSL-Engine-for-ATECC508A)

##Platform Integration
Follow the platform integration instructions found [here](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/ATECC508A:-Platform-Integration)

##Unit Tests
Unit testing is provided for both integration of the ATECC508A device and OpenSSL Examples.  
For details see:
[Platform Integration Tests](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/Tests:-ATECC508A-Platform-Integration)
[OpenSSL Engine Tests & Examples](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/Tests:-OpenSSL-Tests-and-Examples)

Source-Level Documentation
Full Doxygen source-level documentation is provided.
See: /docs/doxygen/html/index.html

##Web Server Setup
The OpenSSL Engine for ATECC508A can also be configured. 
See Details [here](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/Web-Server-For-The-Web-Browser).

##Wiki Topics:
- [Linux Development Setup](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/Linux:-Development-Setup)
- [Compiling on Linux](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/Linux:-Compile-OpenSSL-Engine-for-ATECC508A)
- [Debugging on Linux](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/Linux:-Debugging)
- [ATECC508A Integration](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/ATECC508A:-Platform-Integration)
- [ATECC508A Certificate Provisioning](http://www.microchip.com/developmenttools/productdetails.aspx?partno=at88ckeccroot)
- [Tests and Examples](https://github.com/MicrochipTech/cryptoauth-openssl-engine/wiki/Tests:-OpenSSL-Tests-and-Examples)


