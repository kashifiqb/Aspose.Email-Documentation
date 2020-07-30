---
title: Aspose.Email for Java 20.4 Release Notes
type: docs
weight: 30
url: /java/aspose-email-for-java-20-4-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes information for Aspose.Email for Java 20.4.

{{% /alert %}} 
## **All Changes**

|**Key**|**Summary**|**Category**|
| :- | :- | :- |
|EMAILNET-39783|Support for the ability to Ignore exceptions|Enhancement|
|EMAILNET-39786|Get message infos by unique identifiers for Pop3Client and ImapClient|Enhancement|
|EMAILJAVA-34684|Message fails to process with ArgumentException|Bug|
|EMAILNET-39799|Space getting removed while saving OFT to MSG|Bug|
|EMAILNET-39797|ArgumentOutOfRangeException occurs when loading MailMessage from an html file|Bug|
|EMAILNET-39773|Filtering downloaded messages using ImapQueryBuilder fails|Bug|
|EMAILNET-39776|Unable to download message list|Bug|
|EMAILNET-39770|System.ArgumentOutOfRangeException while loading a MSG|Bug|
|EMAILNET-39764|How to set description(body) for modified occurence|Bug|
|EMAILNET-39790|ReplyMessageBuilder.buildresponse fails while building a response if attachments are present|Bug|
|EMAILNET-39789|Converted MSG to EML does not have From address|Bug|
|EMAILNET-39792|MSG to EML output wrong (Plain Text)|Bug|
|EMAILNET-39791|ImapClient crashes application even called in try catch|Bug|
|EMAILJAVA-34688|The method ITokenProvider.getAccessToken is not called|Bug|
## **New features**
### **Support for the ability to ignore exceptions**
We have prepared a new functionality to ignore exceptions - **ExceptionManager** class has been added to provide ignore exceptions ability:

{{< highlight java >}}

 public class ExceptionManager

{{< /highlight >}}

**Code examples:**

Set a callback to handle exceptions:

{{< highlight java >}}

 ExceptionManager.setIgnoreExceptionsHandler( new IgnoreExceptionsCallback() {

   //exception path: {Module}\{Method}\{Action}\{GUID}

   //example: MailMessage\Load\DecodeTnefAttachment\64149867-679e-4645-9af0-d46566cae598

   public boolean invoke(AsposeException ex, String path) {

       //Ignore all exceptions on MailMessage.Load

       return path.equals("MailMessage\\Load");

   }

});

{{< /highlight >}}

Or use an **alternative**:

{{< highlight java >}}

 ExceptionManager.setIgnoreAll(true);

{{< /highlight >}}

Also, you can set a callback for ignored **exceptions log**:

{{< highlight java >}}

 ExceptionManager.setIgnoreExceptionsLogHandler( new IgnoreExceptionsLogCallback() {

   public void invoke(String message) {

        System.out.println("=== EXCEPTION IGNORED === " + message);

   }

});

{{< /highlight >}}



The user will be notified, that the exception can be ignored by an error message. For example:

{{< highlight plain >}}

 Exceptioin message:

AsposeArgumentException: properties should not be empty.

If you want to ignore an exception and want to proceed further then you can use:

ExceptionManager.getIgnoreList().add("MailMessage\\Load\\DecodeTnefAttachment\\64149867-679e-4645-9af0-d46566cae598")

Invalid TNEF Attachment will be interpreted as regular attachment.

{{< /highlight >}}