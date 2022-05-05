---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2c1019b0c49857e6d8baf4674603329b543b93b5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207344"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignmentScheduleInstances = await client.api('/roleManagement/directory/roleAssignmentScheduleInstances')
    .get();

```