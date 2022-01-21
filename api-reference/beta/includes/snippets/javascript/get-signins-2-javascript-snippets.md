---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 517922f4a679d9f42d562a2fdeeeaeb347b0e903
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095945"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIns = await client.api('/auditLogs/signins?&$filter=startsWith(appDisplayName,\'Azure\')&top=10')
    .version('beta')
    .filter('startsWith(appDisplayName,\'Azure\')')
    .get();

```