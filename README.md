# Nautobot Base Development Template

Follow the Steps to setup the Development Environment :

```shell
$ git clone git@github.com:RitikRatnawat/Nautobot-Dev-Template.git
$ cd <your-repo-folder-name>
```

After that to start a plugin with following steps:
 1. Change the folder name from "\<your-plugin-name\>" to your plugin name.
 2. Update the __init__.py file in the plugin folder with your plugin name.
 3. Update tasks.py file in the current working directory in which update all occurrences of term "\<your-plugin-name\>" with your plugin name.
 4. Update the PLUGINS list in nautobot_config.py with your plugin name.
 5. Update the pyproject.toml with your plugin name.
 6. Rename the development/creds.example.env with development/creds.env
 7. Update "\<your-plugin-name\>" in development/docker-compose.base.yml with your plugin name.


Now to start the Development Environment, Execute the command:
```shell
$ poetry shell
$ poetry install
$ invoke build debug
```
