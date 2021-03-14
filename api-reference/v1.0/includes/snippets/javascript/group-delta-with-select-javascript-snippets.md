---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5eef6240b43d6a836c472b6c769a3a6a436d9de8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/groups/delta')
    .select('displayName,description,mailNickname')
    .get();

```