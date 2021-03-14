---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d481a22a91641950786f7fcd40f9bc820d6135d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroups = await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .get();

```