---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7170790bae14dae8a505d63c1b380b41efec4a26
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalConnection = {
  name: 'Contoso HR Service Tickets',
  description: 'Connection to index HR service tickets'
};

await client.api('/external/connections/contosohr')
    .version('beta')
    .update(externalConnection);

```