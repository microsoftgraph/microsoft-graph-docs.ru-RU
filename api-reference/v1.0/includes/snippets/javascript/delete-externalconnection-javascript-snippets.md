---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fad59b8cb44d6bc9168e482338306ebf010ed554
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688904"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/external/connections/contosohr')
    .delete();

```