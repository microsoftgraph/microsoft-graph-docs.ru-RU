---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07449d471575ed52b4a303d73f5a64e494c7b4aa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _case = {
  displayName: 'My Case 1 - Renamed',
  description: 'Updated description',
  externalId: 'Updated externalId'
};

await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583')
    .version('beta')
    .update(_case);

```