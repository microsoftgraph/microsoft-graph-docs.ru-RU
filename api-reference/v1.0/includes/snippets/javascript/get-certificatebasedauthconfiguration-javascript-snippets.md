---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aa30dc01a1381d0845a29ca28ebf5d6be5c6cad1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793442"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let certificateBasedAuthConfiguration = await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .get();

```