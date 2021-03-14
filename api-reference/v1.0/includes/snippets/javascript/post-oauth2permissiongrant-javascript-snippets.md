---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cafdab9a7d5c59f5919d672606d05111cd2d30d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
  clientId: 'clientId-value',
  consentType: 'consentType-value',
  principalId: 'principalId-value',
  resourceId: 'resourceId-value',
  scope: 'scope-value'
};

await client.api('/oauth2PermissionGrants')
    .post(oAuth2PermissionGrant);

```