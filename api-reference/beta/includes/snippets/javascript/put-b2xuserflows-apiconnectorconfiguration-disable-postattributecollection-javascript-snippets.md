---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03e0c26707b6a07fef4280ad3803380010a87ff0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664472"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = { };

await client.api('/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref')
    .version('beta')
    .put(identityApiConnector);

```