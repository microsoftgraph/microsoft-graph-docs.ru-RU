---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 504cba96c45442fb5dc68e66cc89a8ff23258eaa02fa40819a8fba8cfe3340c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentRequest = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}')
    .version('beta')
    .get();

```