---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2f855e894d0b07738875f7367c9bf22e6dd4116f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
  displayName: 'displayName-value',
  description: 'description-value',
  visibility: 'visibility-value'
};

await client.api('/administrativeUnits/{id}')
    .version('beta')
    .update(administrativeUnit);

```