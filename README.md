# Nautobot Base Development Template

Follow the Steps to setup the Development Environment :

```shell
$ git clone git@github.com:RitikRatnawat/Nautobot-Dev-Template.git
$ cd <your-repo-folder-name>
```

After that to start a plugin with following steps:
 1. Change the folder name from <your-plugin-name> to your plugin name.
 2. Update the __init__.py file in the plugin folder with your plugin name.
 3. Update tasks.py file in the current working directory in which update all occurrences of term <your_plugin_name> with your plugin name.
 4. At last also update the pyproject.toml with your plugin name.
 5. Change the development/creds.example.env with development/creds.env


Now to start the Development Environment, Execute the command:
```shell
$ poetry shell
$ poetry install
$ invoke start debug
```
