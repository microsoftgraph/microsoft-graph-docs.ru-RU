---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ad6ae78eebb791dc5d13995e78aae9f84948d59
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowApiConnectorConfiguration = await client.api('/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration')
    .expand('postFederationSignup,postAttributeCollection')
    .get();

```