---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 82c74e311ca9950ebda94559940b8d6bf1d28098
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35528909"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  allowPublicClient: false,
  displayName: "New display name"
};

let res = await client.api('/applications/{id}')
    .version('beta')
    .update({application : application});

```