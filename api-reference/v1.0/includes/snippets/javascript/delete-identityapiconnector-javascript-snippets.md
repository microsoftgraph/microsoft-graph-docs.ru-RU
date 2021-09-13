---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 88621e0dcbca1bf7ee662702eabeda4196b822f236a1c576aa142c001b335cc4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/apiConnectors/370eeb68-dfd3-4a47-8160-8824c2358321')
    .delete();

```