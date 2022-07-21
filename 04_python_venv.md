# Module

- It may consist of functions and classes in a python file.

- To identify the module that are classes or function by their naming convensions.

- classes are mentioned as PascelCases

        eg. LinearRegression

- Function name are lowercases

        eg. train_test_split

# Package

- It may consist of multiple module in a folder that contain `__init__.py`.

## Package File Structure

```
sklearn
├── __init__.py
└── model_selection
    ├── __init__.py
    └── _split.py
```

- Eg. `from sklearn.model_selection import train_test_split`

# Package Manager

        A Package Manager or Package Mangement System is collection of packages that enable to install, upgrade and remove the package from computer in a consistant manner.

- Eg. `pip, conda, pipenv, poetry`

# Python Environment

## **Linux or MacOS**

### **Using conda**

---

- Creating Virtual Environment

```bash
conda create --name [env_name] python=3.6
python3 -m venv [env_name]
```

- Activating Environment

```bash
conda activate [env_name]
```

- Deactivate Environment

```bash
conda deactivate
```

### **Using Virtualenv**

---

- Creating Virtual Environment

```bash
virtualenv --python=python3.8 [env_name]
```

- Activating Environment

```bash
source [env_path]/bin/activate
```

- Deactivate Environment

```bash
deactivate
```

## **Windows**

`start` >> `cmd` >> `right click` + `Administration Permission` >> type

```bash
Set-ExecutionPolicy Unrestricted
```

`start` >> `cmd` >> type

```bash
pip install virtualenv
```

### **Using conda**

---

**Creating Virtual Environment**

```bash
conda create --name [env_name] python=3.6
```

**Acitivating Environment**

```bash
conda activate [env_name]
```

**Deactivating Enironment**

```bash
conda deactivate
```

### **Using virtualenv**

---

**Creating Virtual Environment**

```bash
virtualenv --python=python3.8 [env_name]
```

**Acitivating Environment**

```bash
.\[env_name]\Script\Activate.ps1
```

**Deactivating Enironment**

```bash
deactivate
```
