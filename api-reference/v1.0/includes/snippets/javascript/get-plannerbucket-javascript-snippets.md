---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4822346c41bc0453fd4c0c39a67ca64fa9a1e01c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerBucket = await client.api('/planner/buckets/{bucket-id}')
    .get();

```