---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bb41ba36641f5933f06ae520621f6d4ce2244134
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroups = await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .version('beta')
    .get();

```