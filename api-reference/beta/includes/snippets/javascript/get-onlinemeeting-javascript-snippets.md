---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3ed7118b17901977dd23e37bff4ad897ec995f07
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onlineMeetings = await client.api('/communications/onlineMeetings/')
    .version('beta')
    .filter('VideoTeleconferenceId eq \'123456789\'')
    .get();

```