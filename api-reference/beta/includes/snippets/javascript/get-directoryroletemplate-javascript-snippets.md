---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1d17e5db0c442c491813d3e37cef15773fd37030
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoleTemplate = await client.api('/directoryRoleTemplates/{id}')
    .version('beta')
    .get();

```