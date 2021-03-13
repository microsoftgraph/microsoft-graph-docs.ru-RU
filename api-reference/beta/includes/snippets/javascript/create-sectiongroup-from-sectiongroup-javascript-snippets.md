---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 83d5dcc232a58274f9ad05e1a4966d8c3b02c981
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809352"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: 'Section group name'
};

await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .version('beta')
    .post(sectionGroup);

```