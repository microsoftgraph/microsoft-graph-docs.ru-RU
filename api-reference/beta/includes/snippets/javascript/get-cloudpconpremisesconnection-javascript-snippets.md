---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3457ab3061edfed32fdba146e2588577bf1cd7b1cce224e2e36a24b5d29ab99d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57195585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcOnPremisesConnection = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{id}')
    .version('beta')
    .get();

```