---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3bf33dd2defa8f96beebe18adf2922e563768dee
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801235"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageCatalogs = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs')
    .version('beta')
    .get();

```