# Tableau Server Utility Tool


## Description

Simple PyQt5 python application, providing the following three Tableau Server maintenance capabilities:

1. Terminate one or multiple extract jobs
2. Transfer ownership of Workbooks/Data Sources to another user, incl. connection credentials
3. Download Data Sources without data extract

## Setup Virtual Environment

Create virtual environment
```
python3 -m venv tableau-ui
```

Activate environment
```
source tableau-ui/bin/activate
```

Install required python packages
```
pip3 install -r requirements.txt
```

## Launch Application

Run:
```
python3 tableau-server-utility-tool.py
```

## Make Layout Changes

Use included `tableau-server-utility-tool.ui` [Qt Designer](https://build-system.fman.io/qt-designer-download) file to adapt the UI and add additional functionality based on your own needs.

Generate new python file from modified .ui file:
```
pyuic5 tableau-server-utility-tool.ui -o tableau-server-utility-tool-new.py
```

Note that this new file just contains the UI. You will need to copy any application functionality from the original file.
