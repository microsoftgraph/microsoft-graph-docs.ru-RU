---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 46ae2e4742be73a1ab7a53f9ff5fc54868ff4290
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800279"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sitePage = await client.api('/sites/{site-id}/pages/{page-id}')
    .version('beta')
    .get();

```