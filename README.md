org.doctales.ant-contrib
========================

![DOCTALES Logo](https://doctales.github.io/images/doctales-logo-without-subtitle.svg)

[![license](https://img.shields.io/github/license/doctales/org.doctales.ant-contrib)](http://www.apache.org/licenses/LICENSE-2.0)

**org.doctales.ant-contrib** is an abstract base [DITA-OT Plug-in](https://www.dita-ot.org/plugins) for [DITA-OT](http://dita-ot.github.io) that provides the [ant-contrib](http://ant-contrib.sourceforge.net/) library. The Ant-Contrib project is a collection of tasks for Apache Ant. The plug-in is designed to be extended.

# Install

The Ant-contrib plug-in has been tested against [DITA-OT 3.x](http://www.dita-ot.org/download). It is
recommended that you upgrade to the latest version.

## Installing DITA-OT

<a href="https://www.dita-ot.org"><img src="https://www.dita-ot.org/images/dita-ot-logo.svg" align="right" height="55"></a>

The Ant-contrib plug-in is a DITA-OT Plugin for the DITA Open Toolkit.

-   Full installation instructions for downloading DITA-OT can be found
    [here](https://www.dita-ot.org/3.3/topics/installing-client.html).

    1.  Download the `dita-ot-3.3.4.zip` package from the project website at
        [dita-ot.org/download](https://www.dita-ot.org/download)
    2.  Extract the contents of the package to the directory where you want to install DITA-OT.
    3.  **Optional**: Add the absolute path for the `bin` directory to the _PATH_ system variable.

    This defines the necessary environment variable to run the `dita` command from the command line.

```console
curl -LO https://github.com/dita-ot/dita-ot/releases/download/3.3.4/dita-ot-3.3.4.zip
unzip -q dita-ot-3.3.4.zip
rm dita-ot-3.3.4.zip
```

## Installing the Plug-in

-   Run the plug-in installation commands:

```console
dita --install https://github.com/doctales/org.doctales.ant-contrib/archive/master.zip
```

The `dita` command line tool requires no additional configuration.

# Usage

To use the The Ant-Contrib plug-in  simply add a `<require>` element to your own `plugin.xml`

#### `plugin.xml` Configuration

```xml
<plugin id="com.example.dita">
  <require plugin="org.doctales.ant-contrib"/>
</plugin>
```

---

# License

[Apache 2.0](LICENSE) © 2017-2019 DocTales

The Program includes the following additional software components which were obtained under license:

-   ant-contrib.jar - http://ant-contrib.sourceforge.net/ - **Apache 2.0 license**

