---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3c7f5c86fc25f5846f9d0969d5ef78ad33cc0255
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workforceIntegration = await client.api('/teamwork/workforceIntegrations/{workforceintegrationid}')
    .version('beta')
    .get();

```