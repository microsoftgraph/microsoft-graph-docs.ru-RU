---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 48609132e50ffa455862fcadb17fc87169d6ad79
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcUserSetting = {
  '@odata.type': '#microsoft.graph.cloudPcUserSetting',
  displayName: 'Example',
  selfServiceEnabled: false,
  localAdminEnabled: true,
  restorePointSetting: {
    frequencyInHours: 16,
    userRestoreEnabled: true
  }
};

await client.api('/deviceManagement/virtualEndpoint/userSettings')
    .version('beta')
    .post(cloudPcUserSetting);

```