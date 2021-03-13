---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c935ac11926f12a769240eeb60ebad40dc81365
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/items/{item-id}/children')
    .version('beta')
    .expand('thumbnails')
    .get();

```