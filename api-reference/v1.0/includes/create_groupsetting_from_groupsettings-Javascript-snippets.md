---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 18cbef42fe72bd270fcdb2724c3ee70c0ff2c756
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: "displayName-value",
  templateId: "templateId-value",
  values: [
    {
      name: "name-value",
      value: "value-value"
    }
  ]
};

let res = await client.api('/groupSettings')
    .post({groupSetting : groupSetting});

```