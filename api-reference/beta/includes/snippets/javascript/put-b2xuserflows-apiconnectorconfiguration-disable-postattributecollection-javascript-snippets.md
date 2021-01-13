---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a5088d5709e4c75d97d681dfc747ee13d79a53a
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = { };

let res = await client.api('/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref')
    .version('beta')
    .put(identityApiConnector);

```