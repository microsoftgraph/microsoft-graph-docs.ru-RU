---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ee8d8f5411127df557f86a92504569a465eccbc4a25d66595f71cece5f64dd57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57247037"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = new Message();
message.subject = "9/8/2018: concert";
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "The group represents Washington.";
message.body = body;
LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.address = "AlexW@contoso.OnMicrosoft.com";
toRecipients.emailAddress = emailAddress;
toRecipientsList.add(toRecipients);
message.toRecipients = toRecipientsList;
LinkedList<InternetMessageHeader> internetMessageHeadersList = new LinkedList<InternetMessageHeader>();
InternetMessageHeader internetMessageHeaders = new InternetMessageHeader();
internetMessageHeaders.name = "x-custom-header-group-name";
internetMessageHeaders.value = "Washington";
internetMessageHeadersList.add(internetMessageHeaders);
InternetMessageHeader internetMessageHeaders1 = new InternetMessageHeader();
internetMessageHeaders1.name = "x-custom-header-group-id";
internetMessageHeaders1.value = "WA001";
internetMessageHeadersList.add(internetMessageHeaders1);
message.internetMessageHeaders = internetMessageHeadersList;

graphClient.me().messages()
    .buildRequest()
    .post(message);

```