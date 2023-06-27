# AutoEnum
Initial network and web application enumeration script for OSCP and Hack The Box

## Setup Virtual Environment
### Install virtualenv
```pip install virtualenv```

### Create a virtual environment
```virtualenv Enum```

### Activate the virtual environment
```source Enum/bin/activate```

## Prerequisite:
- Run the following commands before executing the script:
    - ``` pip install -r requirements.txt ```
    
## USAGE: 
```
usage: auto_enum.py [-h] {enum,web_recon,info} ...

Script for web reconnaissance and enumeration.

positional arguments:
  {enum,web_recon,info}
    enum                Perform enumeration.
    web_recon           Perform web reconnaissance.
    info                Display information of important tools

options:
  -h, --help            show this help message and exit
```

## Example:
```python auto_enum.py enum -t 192.168.203.50 -o 192.168.203.50 -i tun0```

```python auto_enum.py info```

```python auto_enum.py web_recon -s All -p http://localhost:8080 -u "http://192.168.203.50 test1 test2"'``` 


