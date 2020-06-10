---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 071ac014735582c03874d46fc26428af6a37f9da
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681284"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  @odata.id: "https://graph.microsoft.com/beta/applications/{id}"
};

let res = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications')
    .version('beta')
    .post(application);

```