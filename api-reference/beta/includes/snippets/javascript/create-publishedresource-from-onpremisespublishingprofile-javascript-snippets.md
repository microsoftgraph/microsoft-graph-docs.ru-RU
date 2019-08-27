---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d2b4c5714e500107fc264c58e6a70f7beee84db7
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638378"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const publishedResource = {
    displayName: "New provisioning",
    resourceName: "domain1.contoso.com"
};

let res = await client.api('/onPremisesPublishingProfiles/provisioning/publishedResources')
    .version('beta')
    .post(publishedResource);

```