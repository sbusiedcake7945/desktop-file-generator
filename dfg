#!/usr/bin/python
import os

def create(filename, fileext):
    file=open(f"{filename}.{fileext}", "x")
    file.close()

def read(file):
    file=open(f"{file}", "r")
    print(file.read())
    file.close()


def write(file, text):
    file=open(f"{file}", "w")
    file.write(text)
    file.close()

def edit(file, text):
    file=open(f"{file}", "a")
    file.write(text)
    file.close()

def generatedesktop(filename, appname, _exec, icon, cat):
    create(filename, "desktop")
    write(f"{filename}.desktop", "[Desktop Entry]\n")
    edit(f"{filename}.desktop", f"Name={appname}\n")
    edit(f"{filename}.desktop", f"Exec={_exec}\n")
    edit(f"{filename}.desktop", f"Type=Application\n")
    edit(f"{filename}.desktop", f"Icon={icon}\n")
    edit(f"{filename}.desktop", f"Categories={cat}\n")

def main():
    fn=input("desktop file name(without .desktop): ")
    an=input("app name: ")
    e=input("execute command: ")
    c=input("categories: ")
    i=input("icon(path or name): ")
    generatedesktop(fn, an, e, i, c)

main()
