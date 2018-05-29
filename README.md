## This is the reference code for LatinCash cryptocurrency

* Official homepage:
* Official repository: https://github.com/LatinCash/latincash/
* Official Announcement thread:
* Official Twitter:
* Official Telegram:
* Official Whitepaper:
* Official Block explorer:

## LatinCash Cryptocurrency

LatinCash [LCH] is an ASIC resistant CryptoNightLite V1 algorithm based cryptocurrency. 
Fast transactions & privacy make this coin perfect for rewarding your workers, co-workers and colleagues for a job well done.

- Algorithm: CryptoNightLite V1
- Max. supply: 50,000,000.00
- CryptoNote name: LatinCash
- Ticker: LCH
- Decimal points: 4
- Block time: 120
- Emission speed factor: 20
- P2P port: 20634
- RPC port: 20635


## How to compile

### Compile on Linux Ubuntu 16

**1. Install dependencies**

- run an update

``
sudo apt-get update
``

- get all dependencies

``
sudo apt-get install -y build-essential python-dev gcc g++ git cmake librocksdb-dev libboost-all-dev
``

**2. Get the coin**

``
git clone https://github.com/LatinCash/latincash.git latincash
``

**3. CHMOD**

- navigate to:

``
cd latincash/external/rocksdb/build_tools
``

- execute the following commands:

``
chmod +x build_detect_platform
``

``
chmod +x version.sh
``

**4. Build executables**

- Navigate back to repo folder 

``
cd
``

``
cd latincash
``

- prepare the build

``
mkdir build && cd $_
``

``
cmake ..
``

- Export flags

``
export CXXFLAGS="-std=gnu++11"
``

- Make/Build

``
make
``

_Your executables will be located in `build/src` folder._


### Compile on Windows 7/8/10

**1. Environment**

- Visual Studio 2017 Community Edition with desktop development with C++ and the VC++ v140 toolchain features selected
- Boost 1.59.0, with the installer for MSVC 14

**2. Build**

- From the start menu, open 'x64 Native Tools Command Prompt for vs2017'

``
cd <latincash_directory>
``

``
mkdir build
``

``
cd build
``


-  Set the PATH for Cmake:

``
set PATH="C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\IDE\CommonExtensions\Microsoft\CMake\CMake\bin";%PATH%
``

- Run Cmake:

``
cmake -G "Visual Studio 14 Win64" .. -DBOOST_ROOT=C:/ProgramFiles/boost_1_59_0  
``

- Build:

``
MSBuild LatinCash.sln /p:Configuration=Release /m
``

_Your binaries  will be located in `..\build\src\Release` folder._


### Credits
Cryptonote Developers, Bytecoin Developers, Monero Developers, Forknote Project, TurtleCoin Developers, Worktips Developers
