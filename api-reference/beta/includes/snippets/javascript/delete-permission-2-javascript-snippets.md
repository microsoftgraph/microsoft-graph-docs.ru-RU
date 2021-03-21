---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c97a5fe309fbab9a5cc6b57d3900b025a23bda0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .delete();

```