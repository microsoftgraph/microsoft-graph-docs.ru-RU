---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 09deb6b70ff7fc17c45463ee42764a5963928b2f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35528431"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#Microsoft.OutlookServices.ItemAttachment",
  name: "name-value",
  item: "message or event entity"
};

let res = await client.api('/me/events/{id}/attachments')
    .post({attachment : attachment});

```