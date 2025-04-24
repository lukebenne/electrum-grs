Electrum-GRS - Lightweight Groestlcoin Client
=============================================

### License Information:

-   **License**: MIT License

-   **Author**: Groestlcoin Developers

-   **Language**: Python (>= 3.6)

-   **Homepage**: [groestlcoin.org](https://groestlcoin.org/)

### Download Links:

#### Get the latest release of Electrum-GRS for your platform:

-   `Linux (AppImage) <https://github.com/lukebenne/electrum-grs/releases/download/v4.5.4/electrum-grs-4.5.4-x86_64.AppImage>`_

-   `macOS <https://github.com/lukebenne/electrum-grs/releases/download/v4.5.4/electrum-grs-4.5.4.dmg>`_

-   `Windows <https://github.com/lukebenne/electrum-grs/releases/download/v4.5.4/electrum-grs-4.5.4.exe>`_

Electrum-GRS is a fast, efficient, and secure wallet for the Groestlcoin (GRS) cryptocurrency. It is designed to provide a lightweight solution for users looking to manage their Groestlcoin holdings with ease and reliability.

### Key Features:

-   **Lightweight**: Electrum-GRS does not require downloading the entire blockchain, saving you both time and storage space.

-   **Security**: It offers robust security features, including support for hardware wallets and cold storage.

-   **Customizable**: Users can adjust settings for both privacy and transaction handling, providing flexibility for all types of users.

### Getting Started with Electrum-GRS

Electrum-GRS is written in pure Python, ensuring cross-platform compatibility and ease of use. To get started, you can install the required dependencies and run the application on your system.

#### Install Dependencies:

For the Qt interface, install the Qt dependencies with the following command:

`sudo apt-get install python3-pyqt5`

#### Run without Installation:

If you downloaded the official `.tar.gz` package, you can simply run Electrum-GRS from its root directory without needing to install it:

`./run_electrum_grs`

#### Install System-Wide:

Alternatively, install Electrum-GRS on your system using:

`sudo apt-get install python3-setuptools
python3 -m pip install .[fast]`

This will install Python dependencies without needing the 'packages' directory. The `fast` extra includes some optional but useful dependencies.

#### Cloning from GitHub:

If you cloned the repository, you'll need to compile additional files:

`git clone git://github.com/groestlcoin/electrum-grs.git
cd electrum-grs
python3 -m pip install .[fast]`

Compile the protobuf description file:

`sudo apt-get install protobuf-compiler
protoc --proto_path=electrum_grs --python_out=electrum_grs electrum_grs/paymentrequest.proto`

Optionally, create translations:

`sudo apt-get install python-requests gettext
./contrib/pull_locale`

### Creating Binaries

To create binaries for various platforms, follow the relevant instructions below:

-   **Linux (tarball)**: See <contrib/build-linux/README.md>
-   **Linux (AppImage)**: See <contrib/build-linux/appimage/README.md>
-   **macOS**: See <contrib/osx/README.md>
-   **Windows**: See <contrib/build-wine/README.md>

* * * * *