---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff9c4c22d627bf95ae4c17b3a3d355f2051cf984
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798640"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationRoot = await client.api('/education')
    .get();

```