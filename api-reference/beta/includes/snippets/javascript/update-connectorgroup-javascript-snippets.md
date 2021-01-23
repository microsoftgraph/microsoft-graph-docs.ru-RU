---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8880f918989358f17e1c4787c11ae07924b4981f
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945093"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  name: "Connector Group Demo"

};

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups')
    .version('beta')
    .post(connectorGroup);

```