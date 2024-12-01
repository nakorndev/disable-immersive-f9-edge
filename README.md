# Disable F9 on Microsoft Edge

You can use the registry file [disable_immersive_f9_on_edge.reg](disable_immersive_f9_on_edge.reg) to disable the F9 shortcut on Microsoft Edge.

Please note that you need to have administrative privileges to merge the registry file.

After merging the registry file, you need to restart your Microsoft Edge browser for the changes to take effect.

## Disable more keyboard shortcuts

You can disable more keyboard shortcuts by adding the array of string in reg file.

For example, to disable the "find" on command (Ctrl + F), you can add the following string to the "DisabledCommands" array in the reg file:

```reg
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Edge]
"ConfigureKeyboardShortcuts"="{\"disabled\":[\"immersive_reader_toggle\", \"find\"]}"
```

Reference: https://learn.microsoft.com/th-th/deployedge/edge-learnmore-configurable-edge-commands

## Reference

This page is a reference for disable other keyboard shortcuts on Microsoft Edge.  
[Configure keyboard shortcuts](https://learn.microsoft.com/en-us/deployedge/microsoft-edge-policies#configurekeyboardshortcuts)
