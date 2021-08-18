---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 29f997e08154c993388b990c7b13cd9f0a879f07608ea908c69260224eda2260
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57262277"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentItem attachmentItem = new AttachmentItem();
attachmentItem.attachmentType = AttachmentType.FILE;
attachmentItem.name = "flower";
attachmentItem.size = 3483322L;

graphClient.me().messages("AAMkADI5MAAIT3drCAAA=").attachments()
    .createUploadSession(AttachmentCreateUploadSessionParameterSet
        .newBuilder()
        .withAttachmentItem(attachmentItem)
        .build())
    .buildRequest()
    .post();

```