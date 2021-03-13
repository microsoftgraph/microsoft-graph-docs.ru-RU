---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b745adee559b2dc2295bfe485df7c7ccd3d15459
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789284"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/administrativeUnits/{id}')
    .version('beta')
    .delete();

```