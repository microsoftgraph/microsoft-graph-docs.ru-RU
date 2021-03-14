---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0e3e1f83d9846342f454cd37da954f35b1c8df42
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    driveId: '6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B',
    id: 'DCD0D3AD-8989-4F23-A5A2-2C086050513F'
  },
  name: 'contoso plan (copy).txt'
};

await client.api('/me/drive/items/{item-id}/copy')
    .post(driveItem);

```