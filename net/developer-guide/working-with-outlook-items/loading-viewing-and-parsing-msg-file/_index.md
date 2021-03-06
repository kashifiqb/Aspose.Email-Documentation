---
title: Loading, Viewing and Parsing MSG file
type: docs
weight: 20
url: /net/loading-viewing-and-parsing-msg-file/
---


This topic explains how to load a Microsoft Outlook Message file (*.msg). The [MapiMessage](https://apireference.aspose.com/net/email/aspose.email.mapi/mapimessage) class is used to load MSG files and provides several static loading functions for different scenarios. The following code snippet shows you how to load MSG files from file or from stream.
## **Loading MSG Files**
The following code snippet shows you how to load MSG files.



{{< gist "aspose-com-gists" "6e5185a63aec6fd70d83098e82b06a32" "Examples-CSharp-Outlook-LoadMSGFiles-LoadMSGFiles.cs" >}}
## **Loading from Stream**
The following code snippet shows you how to load file from stream.



{{< gist "aspose-com-gists" "6e5185a63aec6fd70d83098e82b06a32" "Examples-CSharp-Outlook-LoadingFromStream-LoadingFromStream.cs" >}}

Converting EML to MSG preserving embedded EML format

EML files can be loaded into [MapiMessage](https://apireference.aspose.com/net/email/aspose.email.mapi/mapimessage) class by instantiating a [MailMessage](https://apireference.aspose.com/net/email/aspose.email/mailmessage) object and passing it to [MapiMessage.FromMailMessage](https://apireference.aspose.com/net/email/aspose.email.mapi/mapimessage/methods/frommailmessage/index) method. If the EML file contains embedded EML files, use [MapiConversionOptions.PreserveEmbeddedMessageFormat](https://apireference.aspose.com/net/email/aspose.email.mapi/mapiconversionoptions/properties/preserveembeddedmessageformat) to retain the format of embedded EML files. The below code snippet shows how to load EML files into [MapiMessage](https://apireference.aspose.com/net/email/aspose.email.mapi/mapimessage) while preserving the format of embedded EML files.



{{< gist "aspose-com-gists" "6e5185a63aec6fd70d83098e82b06a32" "Examples-CSharp-Email-PreservingEmbeddedMsgFormat-PreservingEmbeddedMsgFormat.cs" >}}
