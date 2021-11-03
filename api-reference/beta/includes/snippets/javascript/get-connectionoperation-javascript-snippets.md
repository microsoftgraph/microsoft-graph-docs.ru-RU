---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 31f7f88ae1e0b1c65446fded39636df485727673
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connectionOperation = await client.api('/external/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323')
    .version('beta')
    .get();

```