# bvh_parser_noboost

This repository originally modified from https://github.com/BartekkPL/bvh-parser

The original was under the apache 2.0 license, however I am releasing my version under the MIT License, which as far as I know is entirely legal.

If I made a mistake in licensing this under the MIT then just know that I also make this available to you under the terms of the Apache 2.0 License as provided in ORIGINAL_LICENSE as well.

My own research seems to suggest that it is safe to license under the MIT as long as I do actually provide a copy of the original's apache license and the source changes (see below)

This means that you shouldn't have to provide source changes or a copy of the Apache License like I did, and my research into the topic seems to suggest that this is correct. As described under the MIT License though, you may need to provide a copyright notice.

I'm not going to sue you if you get it wrong, I don't give one flying fuck what you do with this code.

I am not a lawyer, this is not legal advice, etc.

The original repository's Apache License is provided.

## Source changes as required by Apache 2.0 License:
* Removed Boost dependency
* Removed easylogging dependency
* Included <Iterator>

This version of bvh-parser is much more portable as it does not require the boost library.

You still need the C++ STL though, lol.

I am honestly not sure why bvh-parser originally required boost, it seems to be a useless dependency and it was dead simple to clear out (Literally just changing names, adding .c_str() to a couple places, and changing from bf::ifstream to std::ifstream. Also, I had to #include <iterator> for some reason)


The MIT License, under which you may use the contents of this repository:

Copyright 2019 Geklmin

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.