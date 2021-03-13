---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3c834ee5033c7cb82459514dc504c70bde6724f4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780470"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  addLicenses: [],
  removeLicenses: ['skuId-value-1', 'skuId-value-2']
};

await client.api('/groups/1ad75eeb-7e5a-4367-a493-9214d90d54d0/assignLicense')
    .version('beta')
    .post(group);

```