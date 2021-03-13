---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0fa57f3f0acb86824633ef5c35859fa9a47bbf15
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/groups/{id}/members')
    .version('beta')
    .get();

```