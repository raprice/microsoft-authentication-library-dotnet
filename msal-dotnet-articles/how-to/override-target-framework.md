---
title: Overriding target framework
---

# Overriding target framework

In rare circumstances you might want to override NuGet's algorithm of determining the framework version of MSAL. This is useful if you have a confidential client application and need to target `net5.0-windows10.x` because MSAL uses WinForms on these platforms, which leads to build errors in some environments (e.g. Azure Functions).

Please see https://github.com/bgavrilMS/TfmOverride for a proof of concept on how to do this.