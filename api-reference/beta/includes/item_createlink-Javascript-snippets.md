---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e06611a9dfcf9c4d067818939ad5fb0cc3cfe580
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: "view",
  scope: "anonymous"
};

let res = await client.api('/me/drive/items/{itemId}/createLink')
    .version('beta')
    .post(permission);

```