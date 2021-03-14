---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fe415bf77b2ab3889eb14b99407227c0ac2cdadc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendar = await client.api('/me/calendar')
    .get();

```