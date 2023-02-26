On campus til 5
# Aliases

Aliases in the terminal allow you to create custom shortcuts for frequently used commands or programs. This saves time and improves productivity by reducing the amount of typing required.

### Creating Aliases

To create an alias, open your shell's configuration file (e.g. .bashrc or .zshrc) and add your alias definitions in the format of alias alias_name='command_to_run'. 

Open the file using the command:

 ```code ~./bashrc```

The ~/.bashrc file is a script file that is executed every time you start a new terminal session in Bash. This file is commonly used to set environment variables, define aliases, and customize the Bash shell prompt.

To edit the ~/.bashrc file, you need to open it in a text editor. However, since this file is located in your home directory (~), you may not have the necessary permissions to modify it as a regular user. (sudo if required)

For example, to create an alias for git clone:

```alias gc='git clone'```

Add the alias at the end of the file.

### Using Aliases

To use an alias, simply type the alias name in the terminal and press Enter. For example, to use the gc alias to run git clone:

```gc <repository_url>```

### Applying changes

Once you have made changes to the ~/.bashrc file, you need to save the changes and apply them.

To apply the changes, you can either log out and log back in, or simply run the following command in your terminal:

``` source ~/.bashrc ```

This command will reload the ~/.bashrc file and apply any changes you have made to it.

Note that if you made changes to the ~/.bashrc file using sudo, you will need to use sudo when running the source command, like so:

```sudo source ~/.bashrc```

