---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9be3aa6e37031ff97b4f8d660418305a83976b4a115daf6f44380a0ac07e80a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cloudPcDeviceImage = {
  '@odata.type': '#microsoft.graph.cloudPcDeviceImage',
  displayName: 'Display Name value',
  osBuildNumber: 'OS Build Number value',
  operatingSystem: 'Operating System value',
  version: 'Version value',
  sourceImageResourceId: '/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage'
};

await client.api('/deviceManagement/virtualEndpoint/deviceImages')
    .version('beta')
    .post(cloudPcDeviceImage);

```