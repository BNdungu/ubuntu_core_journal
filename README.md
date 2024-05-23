# Installing pip on Ubuntu Core 

This guide provides step-by-step instructions to install `pip` on Ubuntu Core using Python's built-in `urllib` module.

## Prerequisites

- Ubuntu Core installed on your system.
- Python 3 installed (it is included by default with Ubuntu Core).

## Steps

### Step 1: Download `get-pip.py` Using Python's `urllib`

Use Python's `urllib` module to download the `get-pip.py` script:

```bash
sudo python3 -c "import urllib.request; urllib.request.urlretrieve('https://bootstrap.pypa.io/get-pip.py', 'get-pip.py')"
```

### Step 2: Install `pip`

After downloading the `get-pip.py` script, run it using Python 3 to install `pip`:

```bash
sudo python3 get-pip.py
```

### Step 3: Verify the Installation

Verify that `pip` has been installed correctly by checking its version:

```bash
python3 -m pip --version
```

### Step 4: Install Packages Using `pip`

You can now use `pip` to install Python packages. For example, to install the `requests` library, use the following command:

```bash
sudo python3 -m pip install requests
```

### Step 5: Cleanup

After successfully installing `pip`, you can remove the `get-pip.py` script to clean up:

```bash
rm get-pip.py
```

## Troubleshooting

If you encounter any issues during the installation, ensure that:

1. Python 3 is correctly installed and accessible by running `python3 --version`.
2. The `get-pip.py` script was downloaded without errors.
3. You have the necessary permissions to run the commands with `sudo`.

