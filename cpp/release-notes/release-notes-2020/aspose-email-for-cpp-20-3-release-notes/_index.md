---
title: Aspose.Email for CPP 20.3 Release Notes
type: docs
weight: 30
url: /cpp/aspose-email-for-cpp-20-3-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for Aspose.Email for C++ 20.3.

{{% /alert %}} 

Aspose.Email for C++ 20.3 is based on [Aspose.Email for .NET 20.3](https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+20.3+Release+Notes).
## **New features**
**What is OLM storage?**

**OLM file** is the **storage** file format used in Outlook for Mac. **OLM file** is storing local data, such as emails, contacts, tasks, attachments, notes, calendar data, journal, etc. 

**Note**: OLM file is used only by Mac Outlook. 

**New ways of working with OLM storages**

New API provides you with:

- Streaming interface to **OLMClient**
- Extraction of **OLM** files timeout

**OLMClient** usage example:

{{< highlight cpp >}}

 System::SharedPtr<OlmStorage> storage = System::MakeObject<OlmStorage>(u"SampleOLM.olm");

for (auto folder : System::IterateOver(storage->get_FolderHierarchy()))

{

    System::Console::WriteLine(folder->get_Name());

}

{{< /highlight >}}
## **Features not implemented**
The following features are not implemented in Aspose.Email for C++ 20.3 but they are implemented in [Aspose.Email for .NET 20.3](https://docs.aspose.com/display/emailnet/Aspose.Email+for+.NET+20.3+Release+Notes):

- Microsoft Graph REST API v1.0
- Exchange WebDav API
## **API Resources**
The following API resources can be of help to you in getting started with Aspose.Email API.

- [Product Documentation](/email/cpp/home/) – Provides detailed examples of working with the API
- [API Reference Guide](https://www.aspose.com/api/cpp/email) – Details all the namespaces and classes of the API
- [GitHub Examples](https://github.com/aspose-email/Aspose.Email-for-C) – Provides ready to run API example
- [Support Forum](https://forum.aspose.com/c/email) – Write to us if you have any query or inquiry about the API