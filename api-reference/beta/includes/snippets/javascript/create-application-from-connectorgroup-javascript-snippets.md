---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9e13c2dd81eb87208e27d8303f75ac40da1025de
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = Content-type: application/json
Content-length: 30

{
  @odata.id: "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
};

let res = await client.api('/applications/{id}/connectorGroup/$ref')
    .version('beta')
    .put(connectorGroup);

```