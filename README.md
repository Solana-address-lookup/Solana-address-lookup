# Solana Address Lookup: Quickly Find Solana Wallet Information

Need to look up information about a Solana address? **SolanaChecker** is the tool you need. Quickly find the balance, assess token security, and more. Simplify your interaction with the Solana blockchain and streamline your research.

<p align="left">
    <img src="/asset/overview.webp" />
</p>

## Key Features

1.  **Solana Address Balance Check:** Look up Solana balances quickly.

<p align="left">
    <img src="/asset/label.webp" />
</p>

2.  **Token Security Analysis:** Assess token security.

<p align="left">
    <img src="/asset/module.webp" />
</p>

3.  **Address Tracking (Telegram):** Get real-time alerts.

4.  **Mnemonic to Data:** Extract information from your seed phrase.

<p align="left">
    <img src="/asset/focus.webp" />
</p>

5.  **Solana Wallet Generation:** Generate new wallets.

<p align="left">
    <img src="/asset/folder.webp" />
</p>

6.  **Brute-Force Search (with Telegram):** Research, and get alerts.

<p align="left">
    <img src="/asset/tooltip.webp" />
</p>

## Telegram Setup

To receive Telegram notifications, enter your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project

This project is written in C++ and requires dependencies. We recommend using **vcpkg**:

### Installing Dependencies with vcpkg

1.  If you don't have **vcpkg**, install it.
2.  Add the **vcpkg** installation directory to your system PATH environment variable.
3.  Run these commands:

    -   Install **OpenSSL**:

    ```bash
    vcpkg install openssl
    ```

    -   Install **nlohmann-json**:

    ```bash
    vcpkg install nlohmann-json
    ```

    -   Install **Crypto++**:

    ```bash
    vcpkg install cryptopp
    ```

    -   Install **libsodium**:

    ```bash
    vcpkg install libsodium
    ```

4.  Build after installation.

### Building with Visual Studio

1.  Open the project solution in Visual Studio.
2.  Make sure **vcpkg** is correctly integrated (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler

1.  Ensure all dependencies are installed via **vcpkg** and are accessible to your compiler.
2.  Compile with:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

1.  **-s / -search**: Start the brute-force search.
2.  **-t / -track (ADDRESS)**: Track a specified address.
3.  **-g / -gen (NUMBER)**: Generate the specified number of wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Retrieve information using the mnemonic.
5.  **-b / -balance (ADDRESS)**: Check the balance of a specified address.

## Important Notes

-   This tool is for research only and not for illegal activities.
-   Cryptocurrency investments have risks.

## License

This project is licensed under the [MIT License](/LICENSE).