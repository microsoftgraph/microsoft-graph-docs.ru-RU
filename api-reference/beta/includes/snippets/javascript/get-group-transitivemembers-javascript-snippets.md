---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 49af118e0b1194b1c70ceb0236280e1062270001
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMembers = await client.api('/groups/{id}/transitiveMembers')
    .version('beta')
    .get();

```