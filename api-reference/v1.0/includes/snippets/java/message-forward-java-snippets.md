---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dec1c282139b41c43f825b370dc5c129bf23d44b
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "37429207"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "name-value";
emailAddress.address = "address-value";
toRecipients.emailAddress = emailAddress;

toRecipientsList.add(toRecipients);

graphClient.me().messages("{id}")
    .forward(toRecipientsList,null,comment)
    .buildRequest()
    .post();

```