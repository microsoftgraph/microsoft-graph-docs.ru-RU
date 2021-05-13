---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dada5aea392a588d3791c1175ef6fd55675b75aa
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475158"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignmentSchedules = await client.api('/roleManagement/directory/roleAssignmentSchedules')
    .version('beta')
    .get();

```