---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4b77ce0c544fef86cb87669b00757e245c34291c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803946"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = { };

await client.api('/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref')
    .version('beta')
    .put(identityApiConnector);

```