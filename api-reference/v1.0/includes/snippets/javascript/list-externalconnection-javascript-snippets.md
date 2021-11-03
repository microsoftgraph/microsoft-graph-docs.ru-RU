---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fde01944780c2dec75cce65aafb256023e77f135
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696848"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connections = await client.api('/external/connections')
    .get();

```