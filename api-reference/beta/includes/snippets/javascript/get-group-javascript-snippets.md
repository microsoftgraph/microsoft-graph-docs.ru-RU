---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 43ebeba990955a66630d7689b4a50881b3eb9469
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/termStore/groups/{groupId}')
    .version('beta')
    .get();

```