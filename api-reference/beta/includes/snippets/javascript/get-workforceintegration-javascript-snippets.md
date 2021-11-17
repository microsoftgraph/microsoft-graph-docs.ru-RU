---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0f06b8255cc8977854321f5199a7621acde3022e3b3818239af49f6cee96bc20
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57209543"
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