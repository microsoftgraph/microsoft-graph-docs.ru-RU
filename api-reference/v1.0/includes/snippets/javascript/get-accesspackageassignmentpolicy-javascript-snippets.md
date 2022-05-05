---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 52f393d82bb2b52177149e567c62d7dc6b888c87
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209914"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentPolicy = await client.api('/identityGovernance/entitlementManagement/assignmentPolicies/{accessPackageAssignmentPolicyId}')
    .get();

```