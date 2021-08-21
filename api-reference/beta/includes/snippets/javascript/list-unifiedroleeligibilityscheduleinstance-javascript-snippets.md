---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 19a250777ba1578288af1d5b4975429d4b1dc538610d29dc17322c17e543bd4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57319834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleEligibilityScheduleInstances = await client.api('/roleManagement/directory/roleEligibilityScheduleInstances')
    .version('beta')
    .get();

```