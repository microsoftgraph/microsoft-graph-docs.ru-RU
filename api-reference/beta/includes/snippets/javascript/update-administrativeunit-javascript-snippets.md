---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 905800b37af4b742e1547f943b1de6a76fa66a0e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487633"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
  displayName: "displayName-value",
  description: "description-value",
  visibility: "visibility-value"
};

let res = await client.api('/administrativeUnits/{id}')
    .version('beta')
    .update({administrativeUnit : administrativeUnit});

```