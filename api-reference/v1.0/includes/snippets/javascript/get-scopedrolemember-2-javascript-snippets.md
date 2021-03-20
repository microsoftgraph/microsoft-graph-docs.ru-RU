---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: af1deb730fcaa98861b5ffdecd9810935a83309e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMembers = await client.api('/directory/administrativeUnits/{id}/scopedRoleMembers')
    .get();

```