---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3d27f885ac8f9fc13075490c667776a87a8a6022
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774378"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/bundles/{bundle-id}/children/{item-id}')
    .version('beta')
    .delete();

```