---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 036521711548198ed807e9ad39d78da5cc41c450
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567400"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const uploadSession = {
  AttachmentItem: {
    attachmentType: "file",
    name: "flower",
    size: 3483322
  }
};

let res = await client.api('/me/events/AAMkADU5CCmSAAA=/attachments/createUploadSession')
    .post(uploadSession);

```