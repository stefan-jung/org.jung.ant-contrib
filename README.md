org.jung.ant-contrib
========================

[![license](https://img.shields.io/github/license/stefan-jung/org.jung.ant-contrib)](http://www.apache.org/licenses/LICENSE-2.0)

**org.jung.ant-contrib** is a plugin for the [DITA-OT](https://www.dita-ot.org/plugins) that provides the [ant-contrib](http://ant-contrib.sourceforge.net/) library. The Ant-Contrib project is a collection of tasks for Apache Ant.


## Installing the Plug-in

Install the plugin via the `dita` command.

```bash
dita --install https://github.com/stefan-jung/org.jung.ant-contrib/archive/master.zip
```

The `dita` command line tool requires no additional configuration.

# Usage

To use the Ant-Contrib plug-in  simply add a `<require>` element to your own `plugin.xml`

#### `plugin.xml` Configuration

```xml
<plugin id="com.example.dita">
  <require plugin="org.jung.ant-contrib"/>
</plugin>
```

---

# License

[Apache 2.0](LICENSE) ©2013 Stefan Jung

The Program includes the following additional software components which were obtained under license:

-   ant-contrib.jar - http://ant-contrib.sourceforge.net/ - **Apache 2.0 license**
