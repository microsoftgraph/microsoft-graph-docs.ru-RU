---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 87ac19aaa862ecaa8fd1713ba7ece99d95600911
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration')
    .version('beta')
    .expand('postAttributeCollection')
    .get();

```