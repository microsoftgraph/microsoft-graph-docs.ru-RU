---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e8d8e997333a43b3dd20deab14e102c2cd6e4d7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personInterest = await client.api('/me/profile/interests/{id}')
    .version('beta')
    .get();

```