---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 67294b889b0b8d793e7c81bbddda1d2f126cdc28
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printers = await client.api('/print/printers')
    .get();

```