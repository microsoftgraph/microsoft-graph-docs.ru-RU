---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc6c2085a920506a68377c57b6528bda7e773d899c11cf6f41ab0f61e2bee389
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAuditActivityTypes = await client.api('/deviceManagement/virtualEndpoint/auditEvents/getAuditActivityTypes')
    .version('beta')
    .get();

```