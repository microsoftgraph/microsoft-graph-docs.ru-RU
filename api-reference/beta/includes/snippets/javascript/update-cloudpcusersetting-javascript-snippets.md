---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d695fb1b55f270219485c7fe957d69bf7621ed4f
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcUserSetting = {
  '@odata.type': '#microsoft.graph.cloudPcUserSetting',
  displayName: 'Example',
  selfServiceEnabled: true,
  restorePointSetting: {
    frequencyInHours: 16,
    userRestoreEnabled: true
  },
  localAdminEnabled: false
};

await client.api('/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff')
    .version('beta')
    .update(cloudPcUserSetting);

```