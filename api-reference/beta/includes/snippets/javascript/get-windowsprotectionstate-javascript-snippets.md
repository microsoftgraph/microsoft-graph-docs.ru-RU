---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9b34b90d62fcda4dc202db46242f5dcc672bcd67
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let windowsProtectionState = await client.api('/tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}')
    .version('beta')
    .get();

```