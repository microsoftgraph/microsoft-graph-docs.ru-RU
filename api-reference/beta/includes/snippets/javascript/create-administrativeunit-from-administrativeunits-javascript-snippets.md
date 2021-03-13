---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2c36968def2d412567e058c2185a0de449163dac
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
    displayName: 'Seattle District Technical Schools',
    description: 'Seattle district technical schools administration',
    visibility: 'HiddenMembership'
};

await client.api('/administrativeUnits')
    .version('beta')
    .post(administrativeUnit);

```