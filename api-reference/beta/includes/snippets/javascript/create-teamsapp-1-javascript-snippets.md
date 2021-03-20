---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e05d7c94d38ce3406ddc31eb20b1bc311aecca11
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsApp = [Zip file containing a Teams app package];

await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .post(teamsApp);

```