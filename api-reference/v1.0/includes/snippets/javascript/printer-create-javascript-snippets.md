---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aa10574c15e588976cd72ada55ded00e0b23e834
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772053"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const create = {
  displayName: 'Test Printer',
  manufacturer: 'Test Printer Manufacturer',
  model: 'Test Printer Model',
  physicalDeviceId: null,
  hasPhysicalDevice: false,
  certificateSigningRequest: { 
    content: '{content}',
    transportKey: '{sampleTransportKey}'
  },
  connectorId: null
};

await client.api('/print/printers/create')
    .post(create);

```