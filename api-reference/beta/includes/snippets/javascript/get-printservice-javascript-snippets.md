---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f3828002b1426d3d2a4f26b7f0fdb28fdfd0c415
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printService = await client.api('/print/services/{id}')
    .version('beta')
    .get();

```