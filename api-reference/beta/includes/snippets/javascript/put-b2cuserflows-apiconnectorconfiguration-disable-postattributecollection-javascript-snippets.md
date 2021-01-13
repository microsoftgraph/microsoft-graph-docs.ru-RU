---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 06199509ab7a87d4366269875333ba11eeb1231e
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = { };

let res = await client.api('/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref')
    .version('beta')
    .put(identityApiConnector);

```