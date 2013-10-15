jogl-osgi
=========

OSGi bundle for JOGL library

Notes for myself

1) This is an Eclipse plug-in project, so make sure the tools are installed (General Purpose Tools > Eclipse Plug-in Development Environment)

2) Note the manifest with Bundle-NativeCode. Be careful with the spacing.

3) Windows 8 is not recognized under osname win32 in the manifest so it needs a separate entry.

4) You may need to modify the OSGi container configuration properties file to have this:

org.osgi.framework.bootdelegation=sun.\*, javax.\*, apple.\*

Maybe not the best solution? It works for now.
