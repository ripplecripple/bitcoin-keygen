bitcoin-keygen
==============

Ruby script to generate Bitcoin "brain wallet" from any given STDIN input.

The resulting private key will be written in WIF (Wallet Import Format) to STDOUT.

[Please read the warnings about Brain Wallets](https://en.bitcoin.it/wiki/Brainwallet#Precaution)

** USE AT YOUR OWN RISK **

Example usage:

```
# Generate wallet from a passphrase
echo "Hello World" -n | bitcoin-keygen
=> 5Joj3iFDaoGT1RNykhWDJbwBZ28vA9d55iY4631qmt7pEuygaTy

# Generate wallet from a file with a passphrase in it
echo "Hello World" -n > passphrase.txt
cat passphrase.txt | bitcoin-keygen
=> 5Joj3iFDaoGT1RNykhWDJbwBZ28vA9d55iY4631qmt7pEuygaTy

# Generate wallet from an image on disk
cat image1.jpg | bitcoin-keygen
=> 5KQn311se4ZeDDC2o5uwnHLnZhshMNFYs7w57fh2k1oPwwYoN9V

# Generate wallet from a combination of two images on disk
cat image1.jpg image2.jpg | bitcoin-keygen
=> 5Hzz8CHiD6FCyETGu1X3UeHWqrAbDVKnUag5QQWDTBmGXfjhgDE
```


License
=======

The MIT License (MIT)

Copyright (c) 2013 Potiguar Faga

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
