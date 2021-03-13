---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 020ad11495fd6974616d77876781a4c5a0d55271
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794013"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/me/drives')
    .version('beta')
    .get();

```