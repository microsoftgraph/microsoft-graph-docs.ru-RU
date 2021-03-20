---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7ded8f79af2f79ca17e1647cfc4e10eb1c10b3de
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948691"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsApp = [Zip file containing a Teams app package];

await client.api('/appCatalogs/teamsApps')
    .post(teamsApp);

```