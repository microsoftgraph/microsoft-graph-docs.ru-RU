---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0538644671e6d99696140089dcf4921b8e5d97f7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk')
    .version('beta')
    .delete();

```