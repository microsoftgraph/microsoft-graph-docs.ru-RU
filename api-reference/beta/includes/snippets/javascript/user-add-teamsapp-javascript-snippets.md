---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c4e0a26a7a53754327f308a13b5472f1f03fe317843a7d01e3e6082b9d1c5034
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57310001"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userScopeTeamsAppInstallation = {
   'teamsApp@odata.bind':'https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a'
};

await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps')
    .version('beta')
    .post(userScopeTeamsAppInstallation);

```