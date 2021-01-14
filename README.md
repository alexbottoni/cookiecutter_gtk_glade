# README

Cookiecutter Template for generating a basic C language, GTK and Glade application.

The source code is taken from Chapter 4 of "GTK Glade C Programming Tutorial" by *Programmer's Notes*: [GTK+ 3 Glade C Programming Template Files](https://prognotes.net/2015/07/gtk-3-glade-c-programming-template/).

To generate a basic GTK3 empty application, just cd into your target directory and run cookiecutter as follows.

`cookiecutter https://github.com/alexbottoni/cookiecutter_gtk_glade.git`

You will be asked:
1. The name of the target directory (default: "gtk_glade_app")
2. The name of the main .c file (default: "main")
3. The title of the main GTK window (default: "Main Window")

You must have "cookiecutter" installed to perform this action. You can find it here:

[Cookiecutter at GitHub](https://github.com/cookiecutter/cookiecutter)