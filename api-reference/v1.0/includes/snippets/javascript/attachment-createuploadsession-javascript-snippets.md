---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8f210f08d1e6d878313c2d78264f31a30a425cc4b6d30d650febe9037a72ab42
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57365075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const uploadSession = {
  AttachmentItem: {
    attachmentType: 'file',
    name: 'flower', 
    size: 3483322
  }
};

await client.api('/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession')
    .post(uploadSession);

```