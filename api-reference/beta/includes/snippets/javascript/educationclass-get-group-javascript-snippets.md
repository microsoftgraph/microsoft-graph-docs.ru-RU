---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d73ec1cc022b075ef3a4364f0b4a59866133e72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group')
    .version('beta')
    .get();

```