---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 417762583ac2f6701701d42151d4009a9bb5cc3c
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869942"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentMultiple = {
    displayName: 'NewName',
    description: 'A new roleAssignment'
};

await client.api('/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096')
    .version('beta')
    .update(unifiedRoleAssignmentMultiple);

```