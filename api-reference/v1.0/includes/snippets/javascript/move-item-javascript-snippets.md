---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 93bef2a0cd1f109b18d6dd222bb391caa367e9aab444946b073779abb505feac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57366091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    id: '{new-parent-folder-id}'
  },
  name: 'new-item-name.txt'
};

await client.api('/me/drive/items/{item-id}')
    .update(driveItem);

```