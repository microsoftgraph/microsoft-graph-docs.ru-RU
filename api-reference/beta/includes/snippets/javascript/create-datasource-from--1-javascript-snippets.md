---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bf59e05dbec3819c4e8750771c8ab0875eb2c582
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952097"
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