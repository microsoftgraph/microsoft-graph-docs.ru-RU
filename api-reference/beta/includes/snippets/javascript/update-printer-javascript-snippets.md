---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2f9aa72705d0b3036c64ff0ac2cc988511edb5fb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printer = {
  name: 'PrinterName',
  location: {
    latitude: 1.1,
    longitude: 2.2,
    altitudeInMeters: 3
  }
};

await client.api('/print/printers/{id}')
    .version('beta')
    .update(printer);

```