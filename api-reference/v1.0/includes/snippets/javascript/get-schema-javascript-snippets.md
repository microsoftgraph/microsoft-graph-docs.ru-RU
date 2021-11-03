---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03a0f82ccdef9816b8ebf0337b30c2a417eefbee
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694388"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schema = await client.api('/external/connections/contosohr/schema')
    .get();

```