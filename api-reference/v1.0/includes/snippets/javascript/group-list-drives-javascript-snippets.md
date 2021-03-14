---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dfc8d434a06383e92a36b72a4b5481fcdf819944
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/groups/{groupId}/drives')
    .get();

```