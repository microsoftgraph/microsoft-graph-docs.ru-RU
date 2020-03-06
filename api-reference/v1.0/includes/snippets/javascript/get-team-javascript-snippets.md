---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 59ff2f51c489d5918779e01e83765fe98e054d12
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
   teamsApp@odata.bind:"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
};

let res = await client.api('/teams/{id}/installedApps')
    .post(teamsAppInstallation);

```