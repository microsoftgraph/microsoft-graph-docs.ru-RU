---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c6e6648284cc49b0e5384a918668055201922c67
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#Microsoft.OutlookServices.FileAttachment",
  name: "name-value",
  contentType: "contentType-value",
  isInline: false,
  contentLocation: "contentLocation-value",
  contentBytes: "contentBytes-value"
};

let res = await client.api('/me/messages/{id}/attachments')
    .version('beta')
    .post({attachment : attachment});

```