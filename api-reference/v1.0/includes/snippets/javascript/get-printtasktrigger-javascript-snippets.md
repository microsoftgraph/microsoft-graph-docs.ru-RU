---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cfdc8a33a277c279e598d53b4538d9876659afef07fd59af43a6e0de97b8f116
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTaskTrigger = await client.api('/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}')
    .get();

```