---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 354677163c0683516b7cc407d74d8e3ab4a1954a
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628922"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcBulkRemoteActionResult = {
  managedDeviceIds: ['30d0e128-de93-41dc-89ec-33d84bb662a0', '7c82a3e3-9459-44e4-94d9-b92f93bf78dd'] 
};

await client.api('/deviceManagement/managedDevices/bulkReprovisionCloudPc')
    .version('beta')
    .post(cloudPcBulkRemoteActionResult);

```