---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c91a9e7e44cca159a46e6dbd22e6e153482d2ee7da5aac55cd66edba7d32a9ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052627"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryAudit = await client.api('/auditLogs/directoryAudits/{id}')
    .version('beta')
    .get();

```