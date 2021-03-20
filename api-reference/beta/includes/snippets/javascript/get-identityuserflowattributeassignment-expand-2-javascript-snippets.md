---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 23212c5ea0056f5a578128880b3de6078593e9e4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAttributeAssignments = await client.api('/identity/b2xUserFlows/{id}/userAttributeAssignments')
    .version('beta')
    .expand('userAttribute')
    .get();

```