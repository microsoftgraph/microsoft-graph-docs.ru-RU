---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 640f4b56613af57fd22a98d2c837b2e8b4b81e28
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const listItem = {
  fields: {
    Title: 'Widget',
    Color: 'Purple',
    Weight: 32
  }
};

await client.api('/sites/{site-id}/lists/{list-id}/items')
    .version('beta')
    .post(listItem);

```