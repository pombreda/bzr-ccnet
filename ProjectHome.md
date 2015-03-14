# Introduction #

Bazaar plugin for CruiseControl.NET.
You can use it to define a cc.net sourcecontrol task compatible with bzr. The history is parsed as with other VCS.

# Details #

To use the Bazaar plugin for CruiseControl.NET, copy the ccnet.bzr.plugin.dll file into the directory that the other CruiseControl.NET DLLs are in, and add a project to your ccnet.config that uses Bazaar.
See the ccnet.config.sample file for an example of which fields you should add to the project's configuration.

sample:

```
<sourcecontrol type="bzr">
  <branchUrl>http://build/repo/myproject/trunk</branchUrl>
  <workingDirectory>/tmp</workingDirectory>
  <executable>bzr</executable>
</sourcecontrol>
```

# Thanks #

Original project from Sandy Dunlop. https://code.launchpad.net/~sandy-dunlop/bazaar-ccnet/trunk