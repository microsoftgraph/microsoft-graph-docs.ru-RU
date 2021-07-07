---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b74754f68c3a318a88fc5b57b35a88c3a7c142bf
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316988"
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