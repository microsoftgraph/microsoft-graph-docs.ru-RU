---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7a7a878f469ad659f63eaea2f6ede4ba024bdf09
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799229"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let websites = await client.api('/me/profile/websites')
    .version('beta')
    .get();

```