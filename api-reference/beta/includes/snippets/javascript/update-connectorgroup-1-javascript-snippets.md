---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 40596f77ebfe6e796b887dd8c95709b6e262905f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947093"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  name: 'Connector Group Demo'

};

await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups')
    .version('beta')
    .post(connectorGroup);

```