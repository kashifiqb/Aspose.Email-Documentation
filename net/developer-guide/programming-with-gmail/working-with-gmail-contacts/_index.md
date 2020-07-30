---
title: Working with Gmail Contacts
type: docs
weight: 30
url: /net/working-with-gmail-contacts/
---


Aspose.Email supports working with Gmail contacts. Using the IGmailClient interface, users can retrieve contacts from a Gmail account, create new contacts, and update as well as delete existing contacts. Gmail allows developers to perform all these using its public developer's API. The following user information is required for working with Gmail contacts:
User name, email address, password, client ID, client secret refresh token.
This article shows how to:

- [Access Gmail contacts](http://www.aspose.com/docs/display/emailnet/Working+with+Gmail+Contacts#WorkingwithGmailContacts-AccessGmailContacts).
- [Create new Gmail contacts](http://www.aspose.com/docs/display/emailnet/Working+with+Gmail+Contacts#WorkingwithGmailContacts-CreatingContact).
- [Update existing contacts](http://www.aspose.com/docs/display/emailnet/Working+with+Gmail+Contacts#WorkingwithGmailContacts-UpdatingContact).
- [Delete a contact](http://www.aspose.com/docs/display/emailnet/Working+with+Gmail+Contacts#WorkingwithGmailContacts-DeletingContact).
- [Save contact](http://www.aspose.com/docs/display/emailnet/Working+with+Gmail+Contacts#WorkingwithGmailContacts-SavingContact).
## **Access Gmail Contacts**
Following is a sample application which can be used to access the detail of contacts in all the groups.



{{< gist "aspose-email" "9e8fbeb51a8cbc4129dc71ca8cd55f0b" "Examples-CSharp-Gmail-AccessGmailContacts-AccessGmailContacts.cs" >}}
## **Creating Contact**
The following code snippet shows you how to creating contact.



{{< gist "aspose-email" "9e8fbeb51a8cbc4129dc71ca8cd55f0b" "Examples-CSharp-Gmail-CreateGmailContact-CreateGmailContact.cs" >}}
## **Updating Contact**
Once a contact is retrieved, its attributes can be updated and the contact can be saved back to the Gmail account. The following code snippet shows you how to retrieves contacts from a Gmail account and then modifies one of these which is then saved back.



{{< gist "aspose-email" "9e8fbeb51a8cbc4129dc71ca8cd55f0b" "Examples-CSharp-Gmail-UpdateGmailContact-UpdateGmailContact.cs" >}}
## **Deleting Contact**
In order to delete a Gmail contact, the Gmail client's DeleteContact method is used as shown in the following sample snippet.



{{< gist "aspose-email" "9e8fbeb51a8cbc4129dc71ca8cd55f0b" "Examples-CSharp-Gmail-DeleteGmailContact-DeleteGmailContact.cs" >}}
## **Saving Contact**
Aspose.Email allows saving contact to various output formats such as MSG and VCF. The Save method provides the capability to achieve this. The following code snippet shows you how to save contact.



{{< gist "aspose-email" "9e8fbeb51a8cbc4129dc71ca8cd55f0b" "Examples-CSharp-Gmail-SavingContact-SavingContact.cs" >}}