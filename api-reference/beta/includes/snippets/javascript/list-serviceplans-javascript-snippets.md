---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: edb0de418da4b8a2f5350391d3f88a4f3286e7b1
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePlans = await client.api('/deviceManagement/virtualEndpoint/servicePlans')
    .version('beta')
    .get();

```