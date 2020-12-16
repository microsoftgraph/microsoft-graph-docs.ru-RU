---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 25ce14b9870331f9a3c17b9c456e60ccdd31418b
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692587"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _case = {
    displayName: "My Case 1",
};

let res = await client.api('/compliance/ediscovery/cases')
    .version('beta')
    .post(_case);

```