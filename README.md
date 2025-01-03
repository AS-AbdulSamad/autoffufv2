# autoffufv2

This bash script performs web fuzzing on a list of domains using `ffuf` and a provided wordlist, then outputs the results.

## Prerequisites

Before running the script, you need to install two tools:

1. **ffuf** - Fast web fuzzer.
2. **jq** - Command-line JSON processor.

### Installation

#### 1. Install `ffuf`

For **Debian/Ubuntu-based** systems:

```bash
sudo apt update
sudo apt install ffuf
```

Alternatively, you can download the latest release from the ffuf GitHub page.
#### 2. Install jq

For **Debian/Ubuntu-based** systems:
```bash
sudo apt update
sudo apt install jq
```

### Usage
#### 1. Prepare your files

You need two files:

    A domain file containing a list of domains (one per line).
    A wordlist file for fuzzing (e.g., common directory names like admin, login, etc.).

#### 2. Run the script

Clone the repository and navigate to the script directory
Make sure the script is executable
```bash
chmod +x autoffufv2
```
Run the script using the following command
```bash
./autoffufv2 -d <domain_file> -w <wordlist_file>
```
