# how to find plugins

This can be executed from the "Script" console at https://YOUR_JENKINS_URL/script (assuming you are admin)

```groovy
Jenkins.instance.pluginManager.plugins.each{
  plugin -> 
    println ("${plugin.getShortName()}: ${plugin.getVersion()}")
}
```