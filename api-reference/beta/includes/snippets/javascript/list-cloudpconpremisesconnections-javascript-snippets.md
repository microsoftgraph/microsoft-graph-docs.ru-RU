---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: af6b3ccafd9175034c98a6137ab68c10b4d2f897
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onPremisesConnections = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections')
    .version('beta')
    .get();

```