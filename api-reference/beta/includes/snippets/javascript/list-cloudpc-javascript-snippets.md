---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 84de045bfb399a845bec407146d3cbb2d0f021c8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212002"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPCs = await client.api('/me/cloudPCs')
    .version('beta')
    .get();

```