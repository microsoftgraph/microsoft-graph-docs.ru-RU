---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c84c3f20688acb96b2b3c5b33350745b2eba324f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const refreshSession = {

};

await client.api('/me/drive/items/{id}/workbook/refreshSession')
    .version('beta')
    .post(refreshSession);

```