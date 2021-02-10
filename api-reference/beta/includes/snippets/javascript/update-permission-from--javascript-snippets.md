---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b6aa1e9f954b433d55022bdb72beff89b23a771f
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: ["read"]
};

let res = await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .update(permission);

```