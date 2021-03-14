---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 04593e34efde5e2181b4f36378ebf063aad5d3a6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let listItemVersion = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}?expand=fields')
    .get();

```