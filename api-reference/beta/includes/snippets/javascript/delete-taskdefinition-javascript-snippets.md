---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c7c152f3fd37b446d71906816c7e435040dbc662
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/taskDefinitions/4c6a0f26-8e5d-4bf6-91e6-4a5731adec19')
    .version('beta')
    .delete();

```