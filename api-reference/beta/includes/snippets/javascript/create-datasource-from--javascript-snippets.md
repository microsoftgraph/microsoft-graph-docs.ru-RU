---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bf59e05dbec3819c4e8750771c8ab0875eb2c582
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dataSource = {
    '@odata.type': '#microsoft.graph.ediscovery.userSource',
    email: 'badguy@contoso.com'
};

await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources')
    .version('beta')
    .post(dataSource);

```