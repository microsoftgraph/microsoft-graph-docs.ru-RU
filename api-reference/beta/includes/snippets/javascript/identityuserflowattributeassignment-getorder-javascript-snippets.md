---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d5ae478a01db4923406331202670a162da0c6c02e03463ade5897dd287954e93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57192390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignmentOrder = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/getOrder')
    .version('beta')
    .get();

```